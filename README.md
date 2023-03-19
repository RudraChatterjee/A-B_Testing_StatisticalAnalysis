## A/B_HypothesisTesting_NewWebPage

E-news Express, an online news portal, is looking expand its business by acquiring new subscribers. The company has designed a new landing page to attract new subscribers. This python based project performs exploratory data analysis, data visualization and conducts a no of statistical tests on the customer data to determine key business insights 



## **Business Context**

The advent of e-news, or electronic news, portals has offered us a great opportunity to quickly get updates on the day-to-day events occurring globally. The information on these portals is retrieved electronically from online databases, processed using a variety of software, and then transmitted to the users. There are multiple advantages of transmitting new electronically, like faster access to the content and the ability to utilize different technologies such as audio, graphics, video, and other interactive elements that are either not being used or aren’t common yet in traditional newspapers.

E-news Express, an online news portal, aims to expand its business by acquiring new subscribers. With every visitor to the website taking certain actions based on their interest, the company plans to analyze these actions to understand user interests and determine how to drive better engagement. The executives at E-news Express are of the opinion that there has been a decline in new monthly subscribers compared to the past year because the current webpage is not designed well enough in terms of the outline & recommended content to keep customers engaged long enough to make a decision to subscribe.

[Companies often analyze user responses to two variants of a product to decide which of the two variants is more effective. This experimental technique, known as A/B testing, is used to determine whether a new feature attracts users based on a chosen metric.]

## **Objective**

The design team of the company has researched and created a new landing page that has a new outline & more relevant content shown compared to the old page. In order to test the effectiveness of the new landing page in gathering new subscribers, an experiment was conducted by randomly selecting 100 users and dividing them equally into two groups. The existing landing page was served to the first group (control group) and the new landing page to the second group (treatment group). Data regarding the interaction of users in both groups with the two versions of the landing page was collected. The goal of this project is to explore that data and perform a statistical analysis (at a significance level of 5%) to determine the effectiveness of the new landing page in gathering new subscribers for the news portal by answering the following key questions:

#### 1) Do the users spend more time on the new landing page than on the existing landing page?

#### 2) Is the conversion rate (the proportion of users who visit the landing page and get converted) for the new page greater than the conversion rate for the old page?

#### 3) Does the converted status depend on the preferred language?

#### 4) Is the time spent on the new page the same for the different language users?

## **Data Dictionary**

The data contains information regarding the interaction of users in both groups with the two versions of the landing page.

* **user_id** - Unique user ID of the person visiting the website
* **group** - Whether the user belongs to the first group (control) or the second group (treatment)
* **landing_page** - Whether the landing page is new or old
* **time_spent_on_the_page** - Time (in minutes) spent by the user on the landing page
* **converted** - Whether the user gets converted to a subscriber of the news portal or not
* **language_preferred** - Language chosen by the user to view the landing page


## **Key Findings**

#### Time spent on New page vs old page

![image](https://user-images.githubusercontent.com/50159148/226205517-ac03c8db-ef53-4ba5-b774-151c18af069e.png)

It appears that users spend **greater** time on the NEW page vs OLD page

We performed a one tailed t-test at the 5% significance level. P-value came out to be 0.0001 lower than 0.05.
Hence there is enough statistical evidence to say time spent by users on new landing page is greater than time spent by users on the old landing page

