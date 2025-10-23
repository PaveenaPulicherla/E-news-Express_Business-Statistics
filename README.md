# E-news-Express_Business-Statistics


## Business Context
The rise of electronic news portals has revolutionized how users access global updates—offering faster delivery, multimedia integration, and personalized content. **E-news Express**, a digital news platform, seeks to expand its subscriber base by optimizing user engagement through improved landing page design.

Recent trends show a decline in monthly subscriptions, prompting executives to hypothesize that the current webpage layout and content recommendations may not be compelling enough to retain user attention and drive conversions.

## Objective
To evaluate the effectiveness of a newly designed landing page, the Data Science team conducted an A/B test for following questions:

Do the users spend more time on the new landing page than on the existing landing page?

Is the conversion rate (the proportion of users who visit the landing page and get converted) for the new page greater than the conversion rate for the old page?

Does the converted status depend on the preferred language? [Hint: Create a contingency table using the pandas.crosstab() function]

Is the time spent on the new page the same for the different language users?

The goal is to statistically assess whether the new page improves:
-  Time spent on the page
-  Conversion rate (visitor → subscriber)
-  Engagement across preferred languages

## Analytical Questions
1. Do users spend more time on the new landing page than the old one?
2. Is the conversion rate higher for the new page?
3. Does conversion status depend on the preferred language?
4. Is time spent on the new page consistent across different language users?

## Data Dictionary
| Column Name             | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| `user_id`              | Unique identifier for each website visitor                                  |
| `group`                | Indicates whether the user is in the control or treatment group             |
| `landing_page`         | Specifies whether the user saw the old or new landing page                  |
| `time_spent_on_the_page` | Time (in minutes) the user spent on the landing page                        |
| `converted`            | Whether the user subscribed to the news portal (`yes` or `no`)              |
| `language_preferred`   | Language selected by the user to view the landing page                      |

##  Methodology
- **Exploratory Data Analysis (EDA)**: Distribution checks, outlier detection, and visual summaries
- **Statistical Testing**:
  - Independent t-test for time comparisons
  - Proportion z-test for conversion rates
  - Chi-square test for categorical dependencies
  - ANOVA for multi-group mean comparisons

##  Key Findings
- Users spent significantly more time on the new landing page.
- Conversion rate was higher in the treatment group.
- No statistically significant link between language preference and conversion.
- Time spent on the new page was consistent across language groups.

##  Recommendations
- Roll out the new landing page site-wide to boost engagement and subscriptions.
- Consider language-specific campaigns to enhance user experience.
- Continue A/B testing for iterative improvements in layout and content strategy.
