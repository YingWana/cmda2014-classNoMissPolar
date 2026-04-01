# CMDA 2014 — HW10: Sentiment Lab

This repository hosts the class survey dataset for **HW10: Sentiment and Explore Lab** in CMDA 2014 

---

## Quick Start (R)

```r
library(httr)
library(jsonlite)

url <- "https://raw.githubusercontent.com/YingWana/cmda2014-classNoMissPolar/main/classNoMissPolar.json"
dat <- fromJSON(content(GET(url), as = "text", encoding = "UTF-8"))

head(dat)
dim(dat)
```

---

## Dataset Overview

| | |
|---|---|
| **File** | `classNoMissPolar.json` |
| **Records** | 86 students |
| **Variables** | 43 |
| **Format** | JSON |

---

## Data Dictionary

| Variable | Survey Question / Description |
|---|---|
| `code` | Create an anonymous, unique, numerical 4-digit code that only you would know. It may contain ONLY numbers: e.g., 1876. |
| `age` | What is your age in years? E.g., 19.1 |
| `shoe` | What is your US shoe size? (e.g., 6.5, 12, 7, etc) |
| `siblings` | How many siblings do you have? |
| `expGrade` | What grade do you think you will get in this class? |
| `petLove` | Are you a pet lover? - 0 = get that beast away from me; 100 = I have 12 cats; 50 = whatever, do not care. |
| `extrovert` | Are you an extrovert? - 0 = introvert; 100 = extrovert |
| `cookLove` | Do you like to cook? - 0 = I would rather starve; 100 = I will be on the next Chef Wars TV show |
| `spender` | What is your financial tendency? - 0 = money saver (penny pincher); 100 = money spender |
| `texts` | On average, how many texts do you send per day? |
| `politics` | What is your political affiliation? |
| `macLove` | Where are you on the PC vs Mac scale? - 0 = I am ALL PC; 100 = I am ALL Mac |
| `csLove` | How much do you love Computer Science? - 0=hate; 100=love; 50=ok or do not care |
| `statisticsLove` | How much do you love Statistics? - 0=hate; 100=love; 50=ok or do not care |
| `mathLove` | How much do you love Math? - 0=hate; 100=love; 50=ok or do not care |
| `feelingsVt` | How have you felt about Virginia Tech so far? - 0=hate; 100=love; 50=ok or do not care |
| `steps` | How many steps do you take a day? If you do not know, enter -99. |
| `countries` | How many countries have you visited? |
| `states` | How many US states have you visited? |
| `live` | How many places have you lived? |
| `studyRate` | On average, how many hours per week do you study? |
| `sleepRate` | On average, how many hours per week of sleep do you get? |
| `exerciseRate` | On average, how many hours per week of exercise do you get? |
| `anticSalary` | What annual salary do you anticipate once all of your formal education is complete? |
| `quantGifted` | Do you consider yourself to be quantitatively gifted (e.g., good at math or numerical puzzles or anything to do with numbers)? - 0= I HATE quantitative anything; 100=Quantitative genius |
| `artist` | Do you consider yourself an artist? - 0=not an artist; 100=totally an artist |
| `athlete` | Do you consider yourself an athlete? - 0=NOT an athlete; 100=totally an athlete |
| `major` | What is your major or area of study? - Selected Choice |
| `majorOther` | What is your major or area of study? - Other - Text |
| `yearSch` | What year are you in college or grad school? |
| `analyticCourses` | How many statistics/machine learning/computer science courses have you taken prior to this class? |
| `usaProblem` | Of the following, what is the most pressing problem facing America today? |
| `whyClass` | Of the following, what is the main reason why you are in this class? |
| `excitedClass` | Are you excited about this class? - 0=HECK no; 100=Yippee for this class! |
| `dataBoring` | On a scale from 0 (strongly disagree) to 10 (strongly agree), state how you feel in response to the following statements. - Analyzing data is boring |
| `knowHd` | On a scale from 0 (strongly disagree) to 10 (strongly agree), state how you feel in response to the following statements. - I know the meaning of high-dimensional data. |
| `lackMath` | On a scale from 0 (strongly disagree) to 10 (strongly agree), state how you feel in response to the following statements. - My lack of a mathematical background prevents me from analyzing data. |
| `strengths` | Write 5-10 sentences about your strengths as a student. |
| `gains` | Write 5-10 sentences about what you hope to gain from this class. |
| `polarStr0` | Polarity of `strengths` text — primary lexicon only (0 additional words considered). Computed via `polarity()` from R `qdap` package. |
| `polarStr2` | Polarity of `strengths` text — considering 2 words before and after primary lexicon words. Computed via `polarity()` from R `qdap` package. |
| `polarGains0` | Polarity of `gains` text — primary lexicon only (0 additional words considered). Computed via `polarity()` from R `qdap` package. |
| `polaGains2` | Polarity of `gains` text — considering 2 words before and after primary lexicon words. Computed via `polarity()` from R `qdap` package. |

---

## For Educational Use Only
