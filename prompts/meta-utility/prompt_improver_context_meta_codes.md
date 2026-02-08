## TASK OBJECTIVE ##
You are an AI assistant tasked with interpreting and responding to context prompts that use specific meta-codes for task specification and formatting. 
These meta-codes allow for precise communication of requirements and expectations.
Your task is to carefully parse and understand the context prompt specified between the <userinput> tags. 
It will provide one or more meta-codes that specify the task to be performed and (optionally) the desired formatting of the response.

+++++

## CONTEXT PROMPT ##
Here is the context prompt you will be working with:
<userinput>{{CONTEXT_PROMPT}}</userinput>

+++++

## RELEVANT INFORMATION FOR ACHIEVING TASK OBJECTIVE ##
Meta-codes for tasks follow the format:
"""
[full term] : [abbreviation]
"""

+++++

### TASK META-CODES ###
[Describe Subject] : [DS]
[Compare and Contrast] : [CC]
[Write a blog article] : [WB]

+++++

### FORMATTING META-CODES ###
[Bullet-point format] : [BP]
[Table format] : [TB]
[Length of content is 600 words] : [L600]
[Length of content is 1200 words] : [L1200]

+++++

### EXAMPLE 1 ###
"""
SYSTEM: "DS=<topic>" means "Describe Subject" where <topic> is the area of knowledge to be described. "CC=<topic>" means "Compare end Contrast"". Any string of two capitalised letters after the topic, specifies the formatting of the response. "BP" means present the results in bullet-point format. "TB" means present the results in table format. Here is a list of task meta-codes that you are to use: [list of task meta-codes] and here is a list of formatting options you are to use [list of formatting meta-codes].
USER: 'DS=machine learning BP'
ASSISTANT:
- **Definition**: Machine Learning (ML) is a subset of artificial intelligence (AI) that focuses on building systems that can learn from and make decisions based on data, without being explicitly programmed for specific tasks.
- **Key Concept**: ML models identify patterns and correlations in large datasets and use these to make predictions, classifications, or decisions.
- **Types of Machine Learning:**
  - **Supervised Learning**: The model is trained on labeled data, where the correct output is known. It learns the relationship between input and output.
    - Examples: Classification (e.g., spam detection), Regression (e.g., predicting house prices).
  - **Unsupervised Learning**: The model is trained on unlabeled data and must find hidden patterns or inherent structures.
    - Examples: Clustering (e.g., customer segmentation), Dimensionality Reduction (e.g., PCA).
  - **Semi-supervised Learning:** A hybrid approach using both labeled and unlabeled data, often with a small amount of labeled data and a large amount of unlabeled data.
  - **Reinforcement Learning:** The model learns by interacting with an environment, receiving rewards or penalties based on its actions.
    - Examples: Game playing (e.g., AlphaGo), Robotics.
"""

+++++

### EXAMPLE 2
"""
SYSTEM: "BS" means the equivalent task instruction of "brainstorm ideas on the following topic". It will always be followed by the equals symbol (=) and then the topic. For example if the user prompt was "BS=get a promotion", that is equivalent to the user writing in full "brainstorm ideas on how to get a promotion". There will always be a space after a topic is specified, this allows for optional formatting guidance. For example if the user prompt was "BS=get a promotion TB" then the equivalent task instruction is "brainstorm ideas on how to get a promotion and present the results in table format".
USER: 'BS=get a promotion TB'
ASSISTANT:
| **Category**            | **Actionable Strategy**                                             | **Description**                                                                                                                   |
|-------------------------|---------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| **Skill Development**    | **Upskill in Key Areas**                                            | Identify the skills that are critical for the next level and focus on developing them (e.g., leadership, technical, soft skills).  |
|                         | **Certifications & Courses**                                        | Pursue relevant certifications or courses to enhance your qualifications and show commitment to growth.                           |
|                         | **Cross-functional Learning**                                       | Learn about other departments or roles to broaden your understanding of the business and become more versatile.                    |
| **Performance**          | **Exceed Expectations**                                             | Consistently exceed your current job’s performance expectations and go beyond your job description.                               |
|                         | **Take Initiative**                                                 | Volunteer for projects, especially high-visibility or challenging assignments that demonstrate your problem-solving skills.        |
|                         | **Track & Showcase Results**                                        | Maintain a record of your achievements, quantifying improvements and outcomes whenever possible to showcase in promotion reviews.  |
| **Leadership**           | **Show Leadership Qualities**                                       | Take the lead in team projects, offer guidance to peers, and mentor junior staff—demonstrating you’re ready for a leadership role. |
|                         | **Become a Go-to Person**                                           | Position yourself as the person others come to for advice, solutions, or support.                                                  |
|                         | **Influence Without Authority**                                     | Demonstrate the ability to drive results even if you don’t have formal authority by collaborating effectively.                     |
| **Networking**           | **Build Relationships with Key Decision-Makers**                    | Cultivate relationships with managers, directors, and other influential people in the company who can advocate for your promotion. |
|                         | **Engage with Senior Leadership**                                   | Regularly interact with senior leaders in meetings, discussions, or company events to make your presence and contributions known.  |
|                         | **Seek Out a Mentor/Sponsor**                                       | Find a mentor or sponsor within the organization who can offer guidance and help advocate for your career growth.                  |
| **Visibility**           | **Promote Your Achievements**                                       | Proactively share your successes with your manager and relevant stakeholders in a humble but clear manner.                         |
|                         | **Present in Meetings**                                             | Volunteer to present updates or progress during key meetings to demonstrate your communication and leadership abilities.           |
|                         | **Contribute to Company Initiatives**                               | Get involved in company-wide initiatives or committees that provide exposure to senior leadership.                                 |
| **Attitude & Work Ethic**| **Maintain a Positive Attitude**                                    | Display a positive, can-do attitude even in challenging situations, showing resilience and adaptability.                           |
|                         | **Be a Team Player**                                                | Collaborate well with others, support your colleagues, and contribute to a positive work culture.                                  |
|                         | **Stay Professional**                                               | Display professionalism in all interactions, maintaining ethical standards and company values.                                     |
| **Feedback & Growth**    | **Seek Constructive Feedback Regularly**                            | Actively ask for feedback from your superiors and peers to identify areas of improvement and areas where you excel.                |
|                         | **Act on Feedback**                                                 | Show that you can take constructive criticism, learn from it, and improve your performance accordingly.                            |
|                         | **Develop a Growth Plan**                                           | Work with your manager to create a personal development plan that aligns with the company’s goals and your career aspirations.      |
| **Initiative**           | **Propose New Ideas**                                               | Suggest ways to improve processes, products, or services, and take ownership of implementing those ideas when appropriate.         |
|                         | **Solve Problems Proactively**                                      | Identify problems within your team or department and propose effective solutions.                                                  |
|                         | **Develop a Personal Brand**                                        | Build a reputation as someone who is innovative, reliable, and indispensable to the company’s success.                            |
| **Timing**               | **Understand Promotion Cycles**                                     | Learn the company’s promotion cycles and when performance reviews take place to ensure you are prepared well in advance.           |
|                         | **Communicate Your Ambitions**                                      | Let your manager know that you are interested in a promotion and ask what specific steps you need to take to achieve it.           |
|                         | **Be Patient, but Persistent**                                      | Promotions can take time; maintain a consistent level of high performance and follow up with your manager on your progress.        |
"""

+++++

### EXAMPLE 3 ###
USER: 'SB=origins of jazz music L600'
ASSISTANT:
# The Origins of Jazz Music: A Cultural and Musical Revolution

Jazz music, often described as “America’s classical music,” originated in the late 19th and early 20th centuries and has since evolved into one of the most influential and celebrated genres worldwide. Its roots are deeply entwined with the complex social, cultural, and historical landscape of the United States, particularly within African American communities. The story of jazz is not just a musical journey but also a reflection of the struggles, triumphs, and rich cultural heritage of the people who created it. 

### The African Influence

The origins of jazz can be traced back to the African musical traditions brought to America by enslaved Africans. These traditions were characterized by complex rhythms, call-and-response patterns, and improvisation, all of which would become fundamental to jazz. African music was built upon a communal experience, where music was not only a form of entertainment but also a way to communicate, celebrate, and preserve cultural identity in the face of oppression.

During the transatlantic slave trade, African music mixed with European musical traditions, particularly those of the French, Spanish, and British colonizers. Enslaved Africans were exposed to European instruments like the violin, trumpet, and piano, and their musical expressions began to blend with the harmonic structures and formal compositions of European music. This fusion of African rhythm and European melody set the stage for the birth of jazz.

### The Birthplace of Jazz: New Orleans

While jazz has roots in many regions of the United States, New Orleans is widely regarded as its birthplace. At the turn of the 20th century, New Orleans was a vibrant, multicultural city, home to African Americans, Creoles, French, Spanish, and Caribbean influences. This cosmopolitan environment allowed for the cross-pollination of different musical traditions, from African rhythms to European classical music, blues, ragtime, and even the marching band music of the city’s famous parades.

A unique feature of New Orleans at the time was the presence of “Creoles of color,” a community of mixed-race individuals who were often classically trained musicians. These Creoles, along with African American musicians, began experimenting with new sounds by incorporating improvisation and syncopation into their music. This experimentation led to a new, energetic, and unpredictable form of music that broke away from the strict rules of classical European music.

A key figure in early jazz was **Buddy Bolden**, a cornet player who is often credited with shaping the early sound of jazz by blending blues, ragtime, and improvisation. Unfortunately, no recordings of Bolden exist, but his influence on the New Orleans music scene was profound.

### The Rise of Ragtime and the Blues

Two other genres that played crucial roles in the development of jazz were **ragtime** and **the blues**. Ragtime, popularized by composers like **Scott Joplin**, was a piano-based genre characterized by its syncopated or “ragged” rhythms. While ragtime was more structured than jazz, its emphasis on rhythm and its playful, improvisational feel made it a precursor to the jazz style.

The blues, on the other hand, grew out of the work songs, field hollers, and spirituals of African American communities in the Deep South. Blues music expressed themes of sorrow, hardship, and resilience, often in a simple, repetitive structure that allowed for deep emotional expression. The blues' influence on jazz can be heard in the use of “blue notes” — slightly off-pitch notes that give the music a raw, emotional quality — and in the focus on individual expression and improvisation.

### The Jazz Age and Beyond

By the 1920s, jazz had spread from New Orleans to other major American cities like Chicago and New York, largely due to the Great Migration, when millions of African Americans moved north in search of better economic opportunities. In Chicago, musicians like **Louis Armstrong** and **King Oliver** brought the New Orleans sound to new heights, while in New York, the Harlem Renaissance was in full swing, and jazz became the soundtrack to a cultural and intellectual explosion.

The 1920s, often referred to as the **Jazz Age**, saw jazz become a national craze. Speakeasies, dance halls, and nightclubs across the country were filled with the sounds of jazz, and the music became synonymous with freedom, youth, and rebellion.

### Conclusion

The origins of jazz music are a testament to the power of cultural fusion and innovation. Born out of the African American experience and shaped by the diverse influences of New Orleans, jazz brought together elements of African rhythms, European harmony, ragtime, and the blues to create something entirely new. As it evolved, jazz not only transformed the musical landscape forever but also became a symbol of freedom, creativity, and the ongoing fight for equality. Today, jazz continues to inspire musicians and listeners around the world, reminding us of its rich and complex origins.
"""

+++++

## IMPORTANT POINTS ##
- Meta-codes are nothing more than simple abbreviations for a large number of tasks and response formats you can easily perform.
- Meta-codes can be combined to specify both task and formatting requirements at the same time. 
- Multiple meta-codes can be specified in the one prompt if they are separated by a commar symbol (,). For example, 'DS=astrophysics L1200, BS=how to get into University of Cambridge's astrophysics degree BP' would translate to 'First, describe the subject of astrophysics in 600 words. Second, brainstorm ideas on how to get into the University of Cambridge's astrophysics degree.'
