# **Retail Vibe Analytics**



Audience: Technical and business decision makers 

Dataset: Olist Brazilian E-Commerce (Kaggle) -- loaded into Fabric Lakehouse, ecommerce schema



**Setup: Create and empty Fabric notebook and connect it to the Lakehouse. Open it in VS Code.** 



###### Act 1 -- Orient and Explore (3-5 min)



&#x20; **Prompt 1: Schema Discovery**



&#x20; *I have a set of tables in the Fabric Lakehouse attached to this notebook. They are in the ecommerce schema. Have a*

&#x20; *look and tell me about them.*



&#x20; **Purpose: Show that the AI can introspect the lakehouse, describe tables, row counts, and relationships with zero**

&#x20; **upfront context.**



&#x20; **Prompt 2: Star Schema + KPI Snapshot**



&#x20; *Create a star-style view that joins orders, customers, items, payments, and products. Then generate a KPI snapshot:*

&#x20; *total revenue, total orders, avg order value, avg delivery days, and review score.*



&#x20; **Purpose: Demonstrate data modeling on-the-fly and instant executive summary.**



&#x20; **RiffTrax:** 



&#x20; *We're starting completely cold here. I haven't told it anything about this data -- no data dictionary, no ERD, no*

&#x20; *README. I just pointed it at a schema and said 'go.'*



&#x20; *Normally this is the part of the project where you'd spend the first day or two just getting oriented -- pulling up*

&#x20; *table definitions, writing exploratory queries, maybe drawing an ERD on a whiteboard. Your analyst opens SQL Server*

&#x20; *Management Studio, starts poking around, Slacks you three hours later with 'I think I understand the schema.'*



&#x20; *Instead, we got a complete schema summary and a star join in about 30 seconds. And notice it didn't just list*

&#x20; *columns -- it figured out the relationships and built something you could actually use.*



&#x20; *That KPI snapshot? That's usually the deliverable at the END of a discovery sprint. We just got it as a warmup.* 



\-------------------------------------------------------------------------------------------------------------------



##### Act 2 -- Visual Dashboard (5-7 min)



&#x20; **Prompt 3: Multi-Chart Dashboard**



&#x20; *Create a dashboard-style cell with monthly revenue trend, a state-level heatmap of order volume, and a payment*

&#x20; *method mix donut chart.*



&#x20; **Purpose: Wow moment -- a full dashboard from a single sentence. Great for business stakeholders.**



&#x20; **Prompt 4: Refine and Polish**



&#x20; *Make the revenue trend chart a dual-axis showing both revenue and order count. Add a 3-month rolling average line.*

&#x20; *Use a clean, professional color palette.*



&#x20; **Purpose: Show iterative refinement -- "vibe coding" in action. Proves the tool is conversational, not one-shot.**



&#x20; **RiffTrax:** 



&#x20; *Here's where it gets fun. One sentence, three charts. If you've ever filed a ticket with your BI team that*

&#x20; *said 'Can I get a dashboard for this?' -- you know the answer is usually 'Sure, it's in the backlog, we'll get to it*

&#x20; *in about six weeks.'*



&#x20; *We just skipped the backlog.*



&#x20; *Now watch this next part -- I'm going to ask it to refine the chart. Dual axis, rolling average, better colors. This*

&#x20; *is the part that really matters, because real analytics is never one-and-done. You always look at the first draft*

&#x20; *and go 'actually, can you also show me...'*



&#x20; *That conversational loop -- prompt, review, refine -- that IS the workflow. It's not about getting it perfect on the*

&#x20; *first try. It's about making iteration so cheap that you can actually explore. The old way, every tweak was another*

&#x20; *ticket, another wait. Now it's just another sentence.*



\-------------------------------------------------------------------------------------------------------------------



##### Act 3 -- Business Deep-Dives (7-10 min)



&#x20; **Prompt 5: Customer Segmentation (RFM)**



&#x20; *Build an RFM segmentation (Recency, Frequency, Monetary) for all customers. Assign each customer to a segment like*

&#x20; *Champions, Loyal, At Risk, Lost, etc. Show segment counts and avg revenue per segment in a single visual.*



&#x20; **Purpose: Classic analytics use case that normally takes hours. Shows value for marketing/CRM teams.**



&#x20; **Prompt 6: Delivery Performance Analysis**



&#x20; *Analyze delivery performance: what percentage of orders arrived late vs. early? Which states have the worst on-time*

&#x20; *delivery rates? Show a bar chart of avg delivery delay (actual vs estimated) by state, sorted worst-to-best.*



&#x20; **Purpose: Operations/logistics angle -- appeals to COO types. Uses date math and spatial grouping.**



&#x20; **Prompt 7: Product Category Insights**



&#x20; *What are the top 10 product categories by revenue? For each, show the average review score and average delivery*

&#x20; *time. Highlight any categories where high revenue coincides with low review scores -- those are risk areas.*



&#x20; **Purpose: Cross-functional insight (product + CX + ops). Demonstrates the AI can surface non-obvious business risks.**



&#x20; **RiffTrax:** 



&#x20; ***Now we're getting into the stuff that usually requires a specialist.***



&#x20; *RFM segmentation -- if you've done this before, you know the drill. You pull in a data scientist or a senior*

&#x20; *analyst, they spend a couple days writing the recency/frequency/monetary logic, arguing about quintile cutoffs,*

&#x20; *mapping segments to marketing-friendly names. It's a solid week of work before the CMO sees anything.*



&#x20; *We just did it in one prompt.*



&#x20; *The delivery analysis is the same story but for the ops side of the house. Date math, geographic grouping, sorting*

&#x20; *-- it's not rocket science, but it's the kind of thing that takes a good analyst a solid afternoon to get right. And*

&#x20; *somebody always gets the timezone wrong the first time.*



&#x20; *And this product category view -- this is my favorite. It's cross-cutting. It pulls together revenue, customer*

&#x20; *satisfaction, AND delivery performance into one view. This is the kind of analysis that normally falls through the*

&#x20; *cracks because it crosses team boundaries. Product owns the catalog, CX owns the reviews, ops owns delivery --*

&#x20; *nobody owns the intersection. The AI doesn't care about your org chart. It just connects the dots.*



\-------------------------------------------------------------------------------------------------------------------



###### Act 4 -- Advanced / Predictive (5-7 min)



&#x20; **Prompt 8: Review Sentiment and Drivers**



&#x20; *Analyze review scores: what factors most influence whether a customer leaves a 1-star vs 5-star review? Consider*

&#x20; *delivery time, product category, payment type, and order value. Show a correlation heatmap and summarize key*

&#x20; *drivers.*



&#x20; **Purpose: Shows the AI can do exploratory statistical analysis, not just reporting.**



&#x20; **Prompt 9: Cohort Retention Analysis**



&#x20; *Create a monthly cohort analysis: group customers by their first purchase month, then show what percentage made a*

&#x20; *repeat purchase in subsequent months. Display as a retention heatmap.*



&#x20; **Purpose: Sophisticated analysis that typically requires a data scientist. Big impact for growth/product teams.**



&#x20; **Prompt 10: Revenue Forecasting**



&#x20; *Using the monthly revenue trend, fit a simple forecast model and project revenue for the next 6 months. Show the*

&#x20; *historical data, forecast, and confidence interval on a single chart.*



&#x20; **Purpose: Predictive analytics from a plain-English prompt. Strong closer for exec audiences.**



&#x20; **RiffTrax:**



&#x20; *Okay, now we're in 'this would normally require a data scientist' territory.*



&#x20; *That correlation heatmap? That's the kind of analysis where you'd normally write a project brief, schedule a meeting*

&#x20; *with the data science team, wait for them to finish their current sprint, and get results back in two to three*

&#x20; *weeks. And when you get them back, the first thing you say is 'can you also check if payment type matters?' And the*

&#x20; *cycle starts over.*



&#x20; *The cohort retention heatmap -- this is the gold standard for understanding customer lifecycle. Every subscription*

&#x20; *business lives and dies by this chart. Building one correctly -- handling the date logic, the customer matching, the*

&#x20; *percentage calculations -- that's easily a full day for a strong analyst. Maybe two if the data is messy.*



&#x20; *And the forecast -- look, I want to be honest here. This is a simple model. A real production forecast would need*

&#x20; *more rigor. But here's the thing: 90% of the time, what the business actually needs is a directional answer FAST.*

&#x20; *'Are we trending up or down? Roughly where will we land?' You don't always need a PhD-level model. You need a*

&#x20; *good-enough answer in time to actually act on it. That's what this gives you.*



\-------------------------------------------------------------------------------------------------------------------



###### Act 5 -- Wrap-Up / Freestyle (2-3 min)



&#x20; **Prompt 11: Executive Summary**



&#x20; *Summarize everything we've found into a concise executive briefing: top 5 insights, top 3 risks, and top 3*

&#x20; *recommended actions. Format it as a clean markdown report I could email to leadership. Include an impactful visual for each area.* 



&#x20; **Purpose: Demonstrates the AI can synthesize an entire analysis session into an actionable deliverable.**



&#x20; **Prompt 12: Audience Q\&A / Freestyle**



&#x20; *(Don't show this prompt -- use it live based on audience questions)*



&#x20; *Ask the audience: "What would YOU like to explore in this data?"*



&#x20; **Purpose: Most impressive moment -- live, unscripted analysis driven by the room. Shows this is not canned.**



&#x20; **RiffTrax:** 



&#x20; *So here's the thing -- we just did 30 minutes of analysis. If I asked you to write up an executive summary of*

&#x20; *everything we found, how long would that take? An hour? Two? You'd have to scroll back through everything, pull out*

&#x20; *the key numbers, synthesize it into something a VP would actually read.*



&#x20; *Or... one prompt.*



&#x20; *And now -- this is my favorite part -- I want to turn it over to you. What would YOU want to ask this data? Give me*

&#x20; *a question. Anything. We'll run it live right now.*



&#x20; *Because that's the real point here. This isn't a canned demo with pre-baked answers. This is a general-purpose*

&#x20; *reasoning engine sitting on top of your data. The question you have at 4:47 on a Friday that you'd normally say 'eh,*

&#x20; *I'll file a ticket Monday' -- you can just ask it. Right now. No ticket. No backlog. No waiting.*



&#x20;

