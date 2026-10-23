# US Accident Analysis - Power BI Dashboard

This is a Power BI dashboard I built to understand when, where and why road accidents happen in the US. Most of the data comes from California and covers 2016 to 2019.

You don't need to know Power BI to follow this page. I have explained everything in plain words.

---

## Why I made this

Road accidents are a serious problem, but a big table of numbers is hard to read and even harder to learn from. So I turned the data into three simple dashboard pages with charts, buttons and filters. Click a year, a weather type or a severity level, and the whole page updates.

---

## The numbers at a glance

| What | Value |
|---|---|
| Country | US |
| Cities in the data | 1003 |
| Total accidents | 94K |
| Severe accidents | 1,885 (about 2.01%) |
| Years covered | 2016, 2017, 2018, 2019 |

---

## The three dashboard pages

Put your screenshots in an `images/` folder with the names below, and they will show up here.

### Page 1: When and where do accidents happen?

![Page 1](images/page1.png)

This page has:
- Total accidents by month
- Total accidents by quarter
- Total accidents by day of the month
- Total accidents by city
- Year buttons (2016 to 2019) that filter everything

What I noticed:
- March is the worst month with about 9.1K accidents, and August is close behind at about 9.0K.
- December is the quietest month at about 6.0K.
- The four quarters are quite even. Quarter 3 is slightly the highest at 26.4%, and Quarter 4 the lowest at 23.29%.
- Los Angeles is far ahead of every other city with about 10.9K accidents. Sacramento comes second with 4.5K.
- Across the days of the month, accidents stay between roughly 2.6K and 3.5K a day, so no single day stands out much.

---

### Page 2: Does weather or temperature matter?

![Page 2](images/page2.png)

This page has:
- Total accidents by weather condition
- Total accidents by year (pie chart)
- Accidents and average temperature by month (bars with a line)
- Accidents vs temperature (scatter plot)
- Weather buttons such as Clear, Drizzle, Fog and Haze

What I noticed:
- Most accidents happen in clear weather, about 55K. That doesn't mean clear weather is dangerous. Most days are clear, so most driving happens then.
- Overcast (12K), mostly cloudy (8K) and partly cloudy (6K) come next.
- Average temperature moves from about 53°F in winter to about 77°F in summer.
- Most accidents happen between roughly 55°F and 75°F, which is just normal everyday weather.
- By year, 2016 and 2017 have about 28K each, 2018 is the highest with about 31K, and 2019 has only about 7K. That low number most likely means the 2019 data is incomplete.

---

### Page 3: How serious are the accidents?

![Page 3](images/page3.png)

This page has:
- Accident severity distribution (levels 1 to 4)
- Severe accidents by year for California
- Percentage of severe accidents by city
- Percentage of severe accidents by weather condition
- Severity buttons (1, 2, 3, 4)

What I noticed:
- About 90% of accidents are severity 2, the common and less serious kind.
- Around 7.8% are severity 3, and about 2.01% are severity 4, the most severe.
- Severe accidents by year: 574 in 2016, 612 in 2017, 545 in 2018 and 154 in 2019.
- A few small places like Coachella, Norden and Paynes Creek show 100% severe accidents. Be careful here. These places have very few accidents overall, so even one or two severe ones push the percentage to the top.
- By weather, heavy drizzle (50%) and snow (about 23.5%) have the highest share of severe accidents.

---

## What I used

- Power BI Desktop to build the dashboard
- DAX to create measures like Total Accidents, Severe Accidents, % Severe Accidents and Avg Temperature
- A calendar table to break the data down by year, quarter, month and day
- The US Accidents dataset (`US_Accidents_May19...`) with columns like City, State, Country, Start_Time, End_Time, Severity, Temperature(F) and Weather_Condition

---

## What is in this repository

```
├── US_Accident_Analysis.pbix   # The Power BI dashboard file
├── US_Accidents_May19.csv      # The dataset (if the file size allows)
├── images/
│   ├── page1.png
│   ├── page2.png
│   └── page3.png
├── Dashboard.pdf               # PDF export of all pages
└── README.md
```

---

## How to use it

1. Download or clone this repository.
2. Open the `.pbix` file in Power BI Desktop (it is free from Microsoft).
3. Click the year, weather or severity buttons to filter the data.
4. Click any bar or pie slice and watch the other charts change.
5. If you just want a quick look, open the PDF or the screenshots instead.

---

## Main takeaways

1. Accidents peak in March and August and are lowest in December.
2. Los Angeles has by far the most accidents.
3. Most accidents happen in clear weather and normal temperatures, simply because that is when most people drive.
4. Severe accidents are rare, around 2%, but bad weather like heavy drizzle and snow raises the chance of a severe one.
5. Small cities can show very high severe percentages, so always check the total count before drawing conclusions.

---

## A few things to keep in mind

- 2019 has far fewer records than the other years, so it is not fair to compare it directly with 2016 to 2018.
- The "Severe Accidents by State" chart is filtered to California only.

---

## About me

Your Name
Waleed Farooq

If this project helped you, a star on the repo would be much appreciated.
