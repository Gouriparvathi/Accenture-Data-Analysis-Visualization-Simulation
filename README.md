# Accenture Data Analysis & Visualization Simulation
### Client: Social Buzz
## 1. Project Background
Social Buzz is a rapidly scaling social media and content creation platform founded in 2010 in San Francisco by two engineers from London and San Francisco. With over 500 million monthly active users and a core focus on anonymous, content-driven user engagement, Social Buzz collects vast amounts of unstructured data daily from over 100,000 content posts.

The client is preparing for an IPO and seeks expert support to improve data analysis capabilities, scale efficiently, and adopt best practices in big data management. This 3-month pilot project, led by Accenture, is focused on analyzing content popularity trends and delivering data-driven insights to guide their growth strategy.

## 2. Areas of Insights 
- Content Type Performance:
GIFs and videos consistently lead in performance throughout the year, indicating strong visual engagement preferences.

- ❤️ Sentiment Trends:
Despite the variety of topics, content that evokes positive sentiment yields the highest interaction rates.

- 🐾 Category Impact:
The "Animals" category had the highest total engagement score, suggesting a strong emotional resonance with the audience.

- 📅 Temporal Patterns:
Engagement remains stable throughout the months, with no major dips or spikes—useful for planning year-round content.

### Recommendations

- Focus Marketing on Top-Performing Categories
Invest in targeted campaigns and partnerships within the "Animals," "Science," and "Healthy Eating" categories, which show the highest engagement scores. These categories are proven to resonate strongly with the audience and can drive higher ROI on content investments.

- Allocate More Resources to High-Impact Formats
Prioritize the creation of video and GIF content, which consistently deliver high engagement across months. These formats should be emphasized in upcoming content calendars to sustain and grow user interaction levels.

- Leverage Positive Sentiment to Drive Brand Affinity
Since 56% of overall engagement is tied to positive sentiment, content strategies should include emotionally uplifting narratives, positive messaging, and community-driven storytelling to maintain and boost platform loyalty.

- Audit and Reposition Low-Performing Categories
Categories such as “Public Speaking” and “Veganism” show consistently low engagement. Conduct a qualitative review to identify whether these themes need reframing, better creative execution, or can be phased out in favor of higher-performing topics.

- Build Dynamic Feedback Loops Using Reaction & Sentiment Data
Incorporate real-time sentiment and reaction data into content planning cycles. This will help quickly adapt to shifting audience preferences and fine-tune campaigns based on which topics and formats generate the most positive interactions.

## 3. Project Artifacts
📊 Interactive Power BI Dashboard:[here](Dashboards/SocialBuzz_Analysis.pbix)

📈 Cleaned & Transformed Excel Files:[here](Datasets)

## 4. Data Structure (ERD Diagram)
The data for this project is structured across three main tables:

### Table Descriptions
1. Content
- Content ID (Primary Key): Unique identifier for each uploaded content
- Content Type: Type of the content (e.g., image, text, video)
- Category: Thematic classification of content (e.g., Animals, Technology)
- ⛔ Removed: User ID, URL (not relevant to analysis)

2. Reactions
- Content ID (Foreign Key): Links to Content table
- Datetime: Timestamp of the reaction
- Reaction Type (Foreign Key): Type of reaction recorded, links to ReactionTypes
- ⛔ Removed: User ID (due to missing values)
- ⛔ Removed: Blank Reaction Type rows

3. ReactionTypes
- Reaction Type (Primary Key): Name of the reaction (e.g., LOL, Meh, Angry)
- Score: Numerical measure of how popular a reaction is
- Sentiment: Qualitative sentiment tag — Positive, Neutral, or Negative

### Entity Relationship Diagram (ERD)
<img width="554" alt="image" src="https://github.com/user-attachments/assets/43934348-4560-480b-bb2e-a77307162d31" />

- One-to-many relationship from Content → Reactions
- One-to-many relationship from ReactionTypes → Reactions

### Data Cleaning Summary
Power Query transformations applied:

Contents Table
- Standardized casing in Content Type (e.g., unified "Animals" and "animals")

Reactions Table
- Filtered: Rows with blank Reaction Type
- Renamed: “Type” → “Reaction Type” for clarity

## 5. Executive Summary
This project aimed to extract actionable insights from the massive content engagement data generated by Social Buzz from June 2020 to June 2021. The objective was to uncover patterns in audience behavior and provide actionable insights to optimize content strategy and platform performance.

The analysis revealed that engagement is significantly influenced by both the format and emotional tone of the content. Video and GIF formats emerged as the most engaging, while categories like “Animals,” “Science,” and “Healthy Eating” consistently outperformed others in overall interaction metrics. Positive sentiment drives the majority of user engagement, highlighting the importance of emotionally resonant content.

These findings equip stakeholders with a data-backed roadmap for refining content planning, improving audience targeting, and enhancing return on marketing investments.

## 6. Overview of Findings
- Positive sentiment dominates user engagement, accounting for 56% of interactions.
- GIFs, videos, and photos perform similarly well in terms of overall engagement.
- The top-performing content categories are Animals, Science, and Healthy Eating.
- Most content categories show a similar sentiment distribution, with a majority leaning slightly positive.
- Sentiment trends remained relatively stable across 2020 and 2021, with positive engagement consistently above 50%.

<img width="649" alt="image" src="https://github.com/user-attachments/assets/631a4a6e-7d29-422f-a3b2-f3c89cc6fb13" />

