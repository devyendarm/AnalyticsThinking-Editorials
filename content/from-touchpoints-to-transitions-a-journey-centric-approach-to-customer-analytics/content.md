*Imagine you have to meet your CMO in next half-an hour and you know that you have to give a compelling reason and strategy to correct the 18% week over week drop in conversions. As a quick go to tool, you opened the performance dashboard and vigorously tried to slice KPIs by device, channels, geography but you were still unable to find any compelling reason for 'why conversions declined'?*

KPIs such as bounce rates, sessions, pageviews were the foundation of a digital dashboard for nearly two decades. In general, KPIs are used according to the context of the analysis to measure and report performance. However, they only help us understand ‘what happened’ and not so much to understand ‘why users behave in certain ways or how business outcomes can be achieved.’ As customer journeys have become increasingly complex and businesses are expected to deliver consistent performance improvements every passing quarter or year, the insights expected from data have increased in both volume and complexity. Analysts are expected to answer questions such as,

* Why did conversions drop despite an increase in traffic?

* Why do users abandon their carts even after adding shipping information?

* Why do our most loyal customers suddenly churn?

The question ‘why’ is deceptively simple and greatly influences the business and marketing strategy, but deriving meaningful insights is difficult. The aggregated metrics, KPIs, and dimension combinations that signal health, often hide important behavioral nuances needed to understand and interpret the ‘why.’ The problem is not with the dashboarding platforms or the concept of KPIs. The questions business stakeholders ask have simply evolved beyond what dashboards can answer.

To effectively address business concerns and keep pace with evolving customer expectations, especially when Customer Experience (CX) has become far more fragmented across diverse channels, devices, and asynchronous interactions, the Analytics practice should evolve to look beyond traditional KPIs and structured dashboards toward a journey-centric analysis approach, I call this approach the Journey Explorer. Here is a working reference of Journey Explorer implemented for an Ecommerce site, it can be explored at <https://devyendarm.github.io/JourneyExplorer>.

Journey Analysis as a concept is not new. Traditional analysis was focused only on ‘Progression’ with Funnel and Flow visualization, ignoring the critical causal factors of the journey, such as 'Friction,' 'Detour,' and 'Recovery'. Let’s look at how applying these lenses on a simple Customer Journey for an Ecommerce site helps in getting better insights.

### **1. Progression:&#x20;**&#x49;t focuses on **“**&#x44;&#x6F;**&#x20;**&#x75;sers move forward”.

Image 1: [https://drive.google.com/file/d/17wvnnJux1ZXbe-dC_WdOanmgwy7NrXFQ](https://drive.google.com/file/d/17wvnnJux1ZXbe-dC_WdOanmgwy7NrXFQ/edit)

It tells us whether users are moving forward in the journey as designed or there are stages where users fall off the journey the most, signaling friction at that journey stage, hampering users to move forward in the expected journey flow.

In the Ecommerce site analysis, this was at ‘View Item’ stage, the progression is only 66%, effectively dropping over 30% of users in the journey, clearly there is friction at this stage which is affecting the user’s progression. On the contrary, ‘Add Shipping’ stage has the lowest friction with only 10% of users who added their shipping information ended up not Purchasing, demonstrating high Progression rate, clear indication that designed experience is aligned with the user intent.

### 2. **Friction:&#x20;**&#x49;t focuses on “Where do Users stall?”.

Image 2: <https://drive.google.com/file/d/1LaTEHs3hbnglmwUz0t4_J6k2aJTLBOdu/view?usp=drive_link>

Unlike bounce rates and exit rates, which tell us only where someone left the site, friction analysis tells us where the user hesitated, how long they stayed stuck, and whether they attempted the step multiple times before giving up.

As we saw in our Journey Explorer analysis, friction exists at ‘View Item’ stage related to Product View on the Ecommerce site. There can be many reasons for friction that need to be diagnosed. The diagnosis can be effectively done by applying Micro-events, Time factor and other data slicing aspects depending on the context of Analysis.

Image 3: <https://drive.google.com/file/d/1GQLBYUjfqxEf-G_ma0Y30FfI6SUJcwBN/view?usp=drive_link>

In our analysis the friction was contributed by the errors and time taken by users to complete the action, which can be seen in the Time distribution chart. The reason for longer time to action can be analyzed with Channel, Page, and Micro-Events performed at this particular stage. On further analysis, Micro-events diagnosis helps us understand that most users chose ‘Add items to Wishlist’ rather than ‘Add to Cart’, although this is a favorable action, it is not aligned to direct desired Journey Progression.

These are the actionable challenges that need to be resolved to remove friction in the user’s journey.

 

### 3. **Detour:&#x20;**&#x49;t focuses on “Where do Users go when they get lost?”.

Image 4: <https://drive.google.com/file/d/1GF04Q_bKkezTBLPtYRLxtqP68wLWp28Y/view?usp=drive_link>

It is perhaps one of the most underutilized insights in traditional analytics. When users are not proceeding forward in the journey, they either exit the site or take a detour to some other pages which are not aligned with the desired journey. Detour analysis helps in mapping those alternate paths, revealing whether the users are seeking help, second-guessing their intent, or working around a broken experience. The detour paths often expose UX gaps that surveys or heatmaps rarely surface.

In our analysis, we see users browsing FAQ and Shipping Policy pages at the critical Checkout process, although volume is low, these detours could lead to Abandoned Cart journeys.

### 4. **Recovery:&#x20;**&#x49;t focuses on “Do Users come back?”.

Image 5: <https://drive.google.com/file/d/1z3oXuAg9eqcA4-kjR3Qfgk-hKQ1BOPY4/view?usp=drive_link>

It helps in understanding if the users who detoured were due to a temporary distraction or break in the journey. Behavior of users who detoured and returned is distinctly different from the one who never left, as they demonstrated intent but got distracted. Recovery rates, analyzed alongside the detour paths, give analysts a direct measure of experience resilience and how forgiving is the journey when something goes wrong.

In our analysis, only 38% of the users who detoured recovered back in the journey suggesting a need to enhance the journey experience to improve their resilience.

### **Additional Contributors for Diagnosis:**

Along with the 4 lenses, there can be many contributors that help slice lenses of the customer journey.

These can be:

* **Segments:&#x20;**&#x41;ll users do not follow the same path or journey. There are inherent differences between users, it could be the device they use, their region or gender etc. These differences can be defined as segments of users. Applying these segments to slice the aggregate journey at a specific user group level helps in isolating the noise and distribution buried under averaged or aggregated view. The specific segment level customer journey provides better understanding of the journey performance when analyzed with the lenses of 'Progression,' 'Friction,' 'Detour' and 'Recovery'.

* **Specific Stage-Level:** These are stage-specific diagnostic contributors, in my analysis for Ecommerce the following contributors were applied,

  * **Pages or Top paths:** It helped in understanding what are the top contributing pages at the given stage, these pages played a critical influencing role on user’s action, any page which was expected and not present in the list should be analyzed and optimized to improve the performance.

Image 6: <https://drive.google.com/file/d/1JZzUCXxIelFJHiy1NmYuaWSLV6n-YJ42/view?usp=drive_link>

* **Channels:** The top traffic source view at the journey stage helped in understanding if the volumes at a particular journey stage are greatly influenced by internal site navigation and finding methods or driven by the marketing campaigns.

Image 7: <https://drive.google.com/file/d/1x4rQ2eJj3Uzq3XabePaitOcUsHCfYdHf/view?usp=drive_link>

* **Micro-events:** As we already saw at ‘View Item’ stage while understanding Friction, Micro-events were greatly helpful in understanding if the actions performed by the users are aligned directly to the Journey progression or contributing to Friction, for instance the ‘Add to Wishlist’ action although favorable did not directly influence the journey progression similar to ‘Add to Cart’ action which drives the real business goal.

###

### Conclusion

Journey Explorer can represent a meaningful approach for analysts to conduct customer journey analysis. By shifting the unit of analysis from just pages to transitions in the journey, it brings into focus what aggregate metrics have obscured, the actual experience of the users moving through the journey, making decisions, hitting walls, taking detours, and sometimes recovering to find their way back.\
No single lens makes the Journey Explorer powerful. It is the combination of lenses along with their contributing factors. Progression establishes the baseline. Friction pinpoints where intervention is needed. Detour reveals the path users take when the designed journey fails them. Recovery measures how well the experience holds under real-world conditions. Segment filtering ensures these insights are specific rather than averaged across all users, because behavior that looks uniform at aggregate data level is rarely uniform in practice.

For analysts, Journey Explorer is an additional layer and not a replacement for dashboards, it answers the questions dashboards surface most of the time, but cannot resolve them independently. When a KPI drops, Journey Explorer tells us where the drop originated from in the journey, what did the users do instead, and whether the experience recovered. That is the difference between monitoring performance and understanding the journey.