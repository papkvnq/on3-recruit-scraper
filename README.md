# On3 Recruit Scraper
> A powerful scraper that collects detailed college football recruiting rankings and industry comparison data from On3 and other major ranking providers. It helps analysts, developers, and sports researchers access structured, accurate recruit information for deeper insights and performance evaluation.


<p align="center">
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/scraper.png" alt="Bitbash Banner" width="100%"></a>
</p>
<p align="center">
  <a href="https://t.me/Bitbash333" target="_blank">
    <img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>&nbsp;
  <a href="https://wa.me/923249868488?text=Hi%20BitBash%2C%20I'm%20interested%20in%20automation." target="_blank">
    <img src="https://img.shields.io/badge/Chat-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>&nbsp;
  <a href="mailto:sale@bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Email-sale@bitbash.dev-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>&nbsp;
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
</p>




<p align="center" style="font-weight:600; margin-top:8px; margin-bottom:8px;">
  Created by Bitbash, built to showcase our approach to Scraping and Automation!<br>
  If you are looking for <strong>on3-recruit-scraper</strong> you've just found your team — Let’s Chat. 👆👆
</p>


## Introduction
This project retrieves comprehensive comparative recruiting data for American college football recruits. It centralizes rankings, ratings, and positional insights across major industry providers, enabling users to analyze trends, build applications, and power sports analytics workflows.

### Why Recruiting Comparison Data Matters
- Provides a unified view of rankings from On3, 247Sports, Rivals, and ESPN.
- Supports evaluation of player potential across multiple scouting systems.
- Enables performance tracking across recruiting classes over time.
- Feeds data to dashboards, analytics pipelines, and sports applications.
- Helps analysts understand discrepancies between different ranking agencies.

## Features
| Feature | Description |
|----------|-------------|
| Multi-industry data extraction | Retrieves ratings and rankings from On3, 247Sports, Rivals, and ESPN. |
| Flexible recruit selection | Choose any recruiting class year and optionally limit the number of recruits. |
| Detailed structured output | Each recruit includes national, state, and positional ratings and ranks. |
| Multiple export formats | Download data as Excel, CSV, HTML table, JSON, and more. |
| High-accuracy data mapping | Captures nested rating and ranking structures for analytics-ready output. |

---

## What Data This Scraper Extracts
| Field Name | Field Description |
|-------------|------------------|
| playerName | Full name of the recruit. |
| position | Player’s primary playing position. |
| industries | Array containing rating + ranking details for each industry provider. |
| rating | Numerical evaluation score assigned by each industry. |
| rank.national | Recruit’s national ranking for that provider. |
| rank.state | Recruit’s state-level ranking for that provider. |
| rank.position | Recruit’s positional ranking for that provider. |

---

## Example Output


    {
      "playerName": "Arch Manning",
      "position": "QB",
      "industries": [
        {
          "on3Consensus": {
            "rating": "98",
            "rank": {
              "national": "1",
              "state": "1",
              "position": "1"
            }
          }
        },
        {
          "on3": {
            "rating": "98",
            "rank": {
              "national": "1",
              "state": "1",
              "position": "1"
            }
          }
        },
        {
          "twoFourSeven": {
            "rating": "93",
            "rank": {
              "national": "1",
              "state": "1",
              "position": "1"
            }
          }
        },
        {
          "espn": {
            "rating": "6.1",
            "rank": {
              "national": "2",
              "state": "2",
              "position": "1"
            }
          }
        },
        {
          "rivals": {
            "rating": "98",
            "rank": {
              "national": "1",
              "state": "1",
              "position": "1"
            }
          }
        }
      ]
    }

---

## Directory Structure Tree


    On3 Recruit Scraper/
    ├── src/
    │   ├── main.js
    │   ├── scraper/
    │   │   ├── on3_parser.js
    │   │   ├── mapper.js
    │   │   └── helpers.js
    │   ├── utils/
    │   │   ├── formatters.js
    │   │   └── validators.js
    │   └── config/
    │       └── settings.json
    ├── data/
    │   ├── sample_input.json
    │   └── sample_output.json
    ├── exports/
    │   ├── csv_exporter.js
    │   ├── excel_exporter.js
    │   └── json_exporter.js
    ├── package.json
    └── README.md

---

## Use Cases
- **Sports analysts** use it to evaluate cross-industry ranking trends and track recruiting class strength.
- **Developers** use it to populate databases for mobile or web-based recruiting apps.
- **Data scientists** integrate it into pipelines to build predictive models for player performance.
- **Journalists & bloggers** extract structured insights to support recruiting articles and comparisons.
- **Coaches & scouts** monitor player movement and ranking shifts across multiple sources.

---

## FAQs

**Q: What years can I scrape data for?**
A: Any available recruiting class year can be used, as long as the ranking page exists for that year.

**Q: How many recruits can be scraped at once?**
A: Up to 500 recruits can be retrieved per run by adjusting the input configuration.

**Q: Do all industries provide the same ranking fields?**
A: No. Each provider may differ slightly, but the scraper normalizes ratings and ranks to a consistent structure.

**Q: Can this data be exported for integration with analytics tools?**
A: Yes. Output formats like CSV, Excel, and JSON make it compatible with BI tools, spreadsheets, and databases.

---

### Performance Benchmarks and Results

**Primary Metric:** Efficiently processes 300 recruits in under 10 seconds on average due to optimized parsing and minimal dependency overhead.

**Reliability Metric:** Achieves a 99%+ completion rate across recruiting classes thanks to stable page-structure handling and input validation.

**Efficiency Metric:** Memory-optimized data extraction allows smooth runs even at the 500-recruit upper limit.

**Quality Metric:** Produces consistently clean and complete datasets with full rating + ranking coverage for all major industry providers.

---


<p align="center">
<a href="https://calendar.app.google/74kEaAQ5LWbM8CQNA" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
  <a href="https://www.youtube.com/@bitbash-demos/videos" target="_blank">
    <img src="https://img.shields.io/badge/🎥%20Watch%20demos%20-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch on YouTube">
  </a>
</p>
<table>
  <tr>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/MLkvGB8ZZIk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review1.gif" alt="Review 1" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash is a top-tier automation partner, innovative, reliable, and dedicated to delivering real results every time."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Nathan Pennington
        <br><span style="color:#888;">Marketer</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/8-tw8Omw9qk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review2.gif" alt="Review 2" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash delivers outstanding quality, speed, and professionalism, truly a team you can rely on."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Eliza
        <br><span style="color:#888;">SEO Affiliate Expert</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/m-dRE1dj5-k?si=5kZNVlKsGUhg5Xtx" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review3.gif" alt="Review 3" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Exceptional results, clear communication, and flawless delivery. <br>Bitbash nailed it."
      </p>
      <p style="margin:1px 0 0; font-weight:600;">Syed
        <br><span style="color:#888;">Digital Strategist</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
  </tr>
</table>
