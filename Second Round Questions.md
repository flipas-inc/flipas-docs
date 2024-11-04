* **1.Make a website/landing page for your favorite product/company/bar or band**  
* complexity, style and stack is up to u  
  Output: functional link (on vercel or other)

* **2.Answer these questions please**   
* Output: 1 sentence to 3 paragraphs per question  
*   
* \-Why work for Flipas?

* \-Why computers?

* \-What is your favorite aspect of programming?

* \-What job would u do if you werent allowed to be technical?

* **3.Chose one or more problems and provide your solution and/or reasoning:**  
*   
* **a.Design the architecture to a scalable url shortener including stack**  
* Output: Diagram+1 paragraph explaining it

* **b.Given an array of user profile tags like:**  
* \["JavaScript", "JavaScript", "React", "TypeScript", "react", "REACT"\]  
* **Write a function that:**  
* a) Removes duplicates (case-insensitive)  
* b) Normalizes the casing (first letter uppercase, rest lowercase)  
* c) Returns the sorted result  
* Output: Typescript function that returns in this case: \["JavaScript", "React", "TypeScript"\]  
*   
* **c.You have a chat interface where messages can arrive from multiple sources:**  
* \- WebSocket real-time updates  
* \- REST API initial load  
* \- User input  
*   
* How would you implement a React component that:  
* a) Maintains message order  
* b) Prevents duplicates  
* c) Handles optimistic updates for user messages  
* d) Manages loading states  
*   
* Output: the component structure and key hooks  
*   
  **d.You have a profile search component that filters through thousands of profiles:**  
*   
* type Profile \= {  
*   id: string;  
*   name: string;  
*   labels: string\[\];  
*   location: string;  
*   lastActive: Date;  
* }  
*   
* Users can:  
* \- Search by name  
* \- Filter by multiple labels  
* \- Filter by location  
* \- Sort by last active date  
*   
* How would you implement this to ensure good performance?  
* Discuss your approach and any optimizations you'd make.  
* 

*   
* **e.In Flipas's job matching feature, you need to implement a simple**   
* **recommendation algorithm that matches profiles based on different props:**  
*   
* type UserProfile \= {  
*   skills: Skill\[\];           // e.g., \["React", "TypeScript"\]  
*   jobPreferences: string\[\];  // e.g., \["remote", "full-time"\]  
*   experience: number;        // years  
*   location: string;  
*   languages: string\[\];  
* }  
*   
* Output: a function that:  
* a) Takes a target profile and a list of potential matches  
* b) Returns the top 5 most relevant matches  
* c) Considers skill matching weight as most important  
* d) Implements proper TypeScript types  
* e) Performs efficiently for large datasets  
    
    
    
    
* **f.Your MentorAI system needs to be enhanced with new capabilities:**  
*   
* 1\. Function calling to interact with the user's profile data  
* 2\. Context-aware responses based on user's CV/skills  
* 3\. Multi-modal responses (text \+ structured data)  
*   
*   
* type MentorToolCall {  
*   name: string;  
*   description: string;  
*   parameters: Record\<string, unknown\>;  
* }  
*   
* interface MentorResponse {  
*   message: string;  
*   metadata?: {  
*     suggestedSkills?: string\[\];  
*     relevantJobs?: JobMatch\[\];  
*     confidenceScore?: number;  
*   };  
* }  
*   
    
* Design a system that:  
* a) Registers custom tool calls for the OpenAI assistant  
* b) Handles structured responses with metadata  
* c)Provides value  
* 