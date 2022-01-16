# Power-BI-Assignment-2

### 1. Explain the advantages of Natural Queries in PowerBi with an example?

- It requires no prior knowledge on any querying language like SQL, excel. Querying is carried out using common and natual English language.
- Once dashboard is created and submitted to Business stakeholders, stakeholders find it easy to query on their own in the report submitted by the Analyst Team.
- Power BI shows predictions as user types the query which indeed helps user to query faster and confidently
- It reduces confusion to layman

for example, we may query **"show total sales country wise"**. Power BI understands the query as we type. When we type "show" it lists all the features available. The respected query results are displayed to user/Business stakeholders.

### 2. Explain Web Front End(WFE) cluster from Power BI Service Architecture?

Power BI service Architecture contains two clusters.
- Web Front End cluster (WFE)
- Back end cluster

Web Front End(WFE) cluster manages two important components.
- Initial connection
- User Autentication

Frond end cluster acts as intermediary between client and back end. 

It uses **Azure Traffic Manager (ATM)** to make efficient and quick authentication. It attemps to send user traffic to nearest data center to reduce connection time. The nearest location is found by the DNS record of client attempting to connect.

Once user is connected, he/she can access static content & files. To share these files, Power BI uses another technology called **Azure Content Delivery(ACD)** to efficiently distribute the respective user file contents based on geographic locale.
