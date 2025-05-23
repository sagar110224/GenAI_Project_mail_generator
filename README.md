# Smart_Sales_Email_Generator

Definition: 
Customer: An individual or business that has subscribed to Agentro and uses the platform to promote their product or service.
Prospect: A potential client targeted through the Agentro system, to whom promotional emails will be created and sent.
 
A program was created that:
1.Loads a list of prospects from a CSV file (name, company, email, and a short business description).
2.Uses the company URL (customer’s business) and create the company profile using LLM that can be used to write emails that will be sent to the prospect. 

For each prospect:
1.Uses OpenAI's API to generate a personalized sales outreach email that:
a.Highlights how the customer’s product can benefit the prospect.
b.Reflects understanding of both the customer’s and the prospect’s business.

Simulates email tracking by:
1.Randomly marking some prospects as “no reply.”
2.Automatically generating a follow-up email using open AI. The follow up should be generated by intelligently analyzing the response from the Prospect. For example if the prospect responded with additional information about product and company or prospect responded with date and time for meeting, the response should be drafted accordingly. 

Outputs a CSV with:
Name, company, email, initial email, follow-up status, follow-up email (if any).
