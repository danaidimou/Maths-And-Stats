# Maths-And-Stats Project

A cooking website wants to improve their product page. Up until now they have had a horizontal rail. A UX designer suggested having a vertical one.

The business problem we are trying to solve is figuring out whether the media rail change will affect the user engagement and potentially the sales. 
Improving the product page might be crucial for the company because it influences the user experience. By optimizing the page layout, the company can create a more enjoyable browsing experience, potentially increasing customer satisfaction, loyalty and revenue.
However, drawbacks could include the potential for information overload if too many items are displayed at once, or it might disrupt users accustomed to the horizontal layout. Balancing the presentation of information is important to ensure that the change will have a positive impact. 

The hypothesis we're testing concerns the impact of changing the media rail from horizontal to vertical on a cooking website’s product page. We're assuming that this change would increase the customer engagement and potentially the sales.   
The null hypothesis would be that there is no significant difference in user engagement or sales between the horizontal and vertical layouts.
The alternative hypothesis would be that the vertical media layout significantly affects user engagement compared to the horizontal one.
_______________________________________________________________________________________________________________________________________________________

An A/B test is an effective method for testing hypotheses because it allows for a controlled experiment comparing two versions to see which performs better on specific metrics. It provides clear, quantitative evidence on whether the new variant impacts user engagement or sales, making it a powerful tool for data-driven decision-making.

Another method that could’ve been used is customer surveys.

While A/B testing is an excellent tool for obtaining objective, quantitative data on user behavior in response to specific changes, it can be limited, focusing mainly on the impact of those changes without capturing broader user needs or preferences. On the other hand, customer surveys can provide rich qualitative insights that A/B testing might miss, offering a deeper understanding of user motivations, preferences, and feedback on a wide range of topics.

A/B testing allows for a controlled environment where external variables are minimized, giving a clear picture of direct impacts on user behavior or KPIs. However, this method can be time-consuming and expensive, requiring the right tools and expertise to get meaningful results. In contrast, customer surveys are typically quicker and more cost-effective to deploy, although they come with their own set of challenges such as potential response bias and the complexity of interpreting qualitative data.

One of the key advantages of A/B testing is that it's enabling the collection of statistically significant data from a large number of users. Yet, the insights gained are generally limited to the specific variations being tested. Customer surveys, while offering direct feedback from users and the ability to explore a broader range of questions, may lack subjectivity in responses and lower response rates, which can affect the reliability of the data collected.

So while A/B testing provides precise insights into how changes affect user behavior, it lacks the depth of user understanding that surveys can provide. Surveys, despite their broader scope and direct user feedback capabilities, have issues of subjectivity and potential biases. The choice between the two methods —or the decision to use them both— depends on the specific goals, context, and resources available for your research or data collection.
______________________________________________________________________________________________________________________________________________________

As a primary metric, I chose the 'Number of add to cart'. The orientation change of the product media rail should influence the users engagement and intent to purchase. This metric will directly reflect the initial impact of the media rail orientation change on user behavior, serving as an immediate indicator of user interest and potential intent to purchase.
I chose the 'GMV in $' as a secondary metric in order to understand whether increased add-to-cart actions translate into actual revenue and 'Clicks on media' in order to actually see in which variant the users were more engaged.
One metric missing that could've been of value is the Bounce Rate on Product Pages. It could indicate the percentage of visitors who leave the site after viewing just one page, which can help assess initial user interest and the effectiveness of page content. Other data that could be usefull are surveys and feedback from the users.
_______________________________________________________________________________________________________________________________________________________

After deciding what metrics I wanted to use, I calculated the distribution atributes in order to see if they are normally distributed and noticed that the data in GMV in $ is not normally distributed, since there was some skewness, but since the sample size is large enough to rely on the Central Limit Theorem, I went for the two-sample t-test.

For Number of Add to Cart (Primary Metric):
T-statistic: -8.7774
P-value: 3.517×10 to the power of −18
The negative t-statistic indicates that the mean "Number of Add to Cart" is lower in Variant A compared to Variant B. The extremely small p-value suggests that this difference is statistically significant. We can confidently reject the null hypothesis and conclude that the change to the media rail has a significant impact on the number of items users add to their carts.

"GMV (in $)":
T-statistic: -1.28395
P-value: 0.1993
The negative t-statistic here indicates that the mean GMV is lower in Variant A compared to Variant B. However, the p-value is greater than the typical alpha level of 0.05, indicating that this difference is not statistically significant. Therefore, we cannot reject the null hypothesis for GMV, suggesting that the change in the media rail did not significantly affect the GMV between the two variants.

"Clicks on Media":
T-statistic: 3.17107
P-value: 0.00154
The positive t-statistic indicates that the mean "Clicks on Media" is higher in Variant A compared to Variant B. The p-value is less than 0.05, indicating that this difference is statistically significant. We can reject the null hypothesis, concluding that Variant A leads to significantly more media clicks compared to Variant B.
______________________________________________________________________________________________________________________________________________________

The data shows that Variant B significantly increases the number of add-to-cart actions, a key indicator of user engagement and potential sales. Implementing Variant B across the site could enhance overall performance.  
While Variant B doesn't show a significant difference in GMV now, the increase in add-to-cart actions might lead to higher sales over time. It's also worth noting that Variant A resulted in more clicks on media, indicating that aspects of Variant A could be engaging users in ways that Variant B does not. Therefore, it might be beneficial to deeper dive into the elements that made Variant A more engaging. By doing a segmentation and user journey analysis, we could break down the data by user segments (e.g., new vs. returning users and different demographics) and examining the paths users take on the site, especially how they interact with the media rail and what actions follow those interactions.
