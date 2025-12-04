# Methuen Public Schools Analysis - Data Sources & Methodology

## Independent Verification Guide
**Analysis Date:** December 4, 2025  
**Analyst:** Claude (Anthropic AI)  
**District Code:** 01810000  

---

## DATA SOURCES

### 1. MA DESE Accountability Report 2025
**URL:** https://profiles.doe.mass.edu/accountability/report/district.aspx?linkid=30&orgcode=01810000&orgtypecode=5  
**Accessed:** December 4, 2025  
**Data Updated:** September 29, 2025 (per DESE)

### 2. MCAS Achievement Levels 2025
**URL:** https://profiles.doe.mass.edu/mcas/achievement_level.aspx?orgcode=01810000&orgtypecode=5  
**Accessed:** December 4, 2025  
**Data Updated:** September 29, 2025 (per DESE)

### 3. Education Spending Data
**Source File:** `/home/claude/ma_taxpayer_report/data/education_spending.csv`  
**Original Source:** MA DESE Per Pupil Expenditure Report

---

## RAW DATA EXTRACTED

### Spending Data (from education_spending.csv)
```
District: Methuen
District Code: 1810000
In-District Expenditures: $108,651,638.60
In-District FTE: 6,574.1
In-District Per Pupil: $16,527.23
Total Expenditures: $131,233,198.80
Total FTE: 7,068.8
Total Per Pupil: $18,565.13
```

**Calculation - Comparison to US Average:**
- US Average Per Pupil (2022-23): ~$15,633 (NCES)
- Methuen: $18,565
- Difference: ($18,565 - $15,633) / $15,633 = 18.8% ≈ 19% above US average

### MCAS Proficiency Rates - Grades 3-8 (Spring 2025)
| Subject | Meeting/Exceeding | State Average | Difference |
|---------|-------------------|---------------|------------|
| ELA | 30% | 42% | -12 pts |
| Math | 27% | 41% | -14 pts |
| Science | 27% | 42% | -15 pts |

**Source rows from DESE MCAS Achievement Level report:**
```
GRADES 03 - 08 - ENGLISH LANGUAGE ARTS: 30% M/E (State: 42%)
GRADES 03 - 08 - MATHEMATICS: 27% M/E (State: 41%)
GRADES 05 & 08 - SCIENCE AND TECH/ENG: 27% M/E (State: 42%)
```

### MCAS Proficiency Rates - Grade 10 (Spring 2025)
| Subject | Meeting/Exceeding | State Average |
|---------|-------------------|---------------|
| ELA | 33% | 51% |
| Math | 25% | 45% |
| Science | 36% | 46% |

### Year-over-Year MCAS Score Changes (2024 → 2025)

**High School (Grade 10):**
| Subject | 2024 Score | 2025 Score | Change |
|---------|------------|------------|--------|
| ELA | 494.9 | 489.5 | -5.4 |
| Math | 490.4 | 486.3 | -4.1 |
| Science | 493.2 | 491.7 | -1.5 |

**Grades 3-8:**
| Subject | 2024 Score | 2025 Score | Change |
|---------|------------|------------|--------|
| ELA | 486.6 | 487.3 | +0.7 |
| Math | 486.9 | 486.3 | -0.6 |
| Science | 485.4 | 485.2 | -0.2 |

**Source:** DESE Accountability Report "English language arts achievement" and "Mathematics achievement" tables

### Accountability Targets Met
```
2024 Annual criterion-referenced target percentage: 46%
2025 Annual criterion-referenced target percentage: 39%
Cumulative (weighted): (46% × 40%) + (39% × 60%) = 18.4% + 23.4% = 41.8% ≈ 42%
Classification: "Moderate progress toward targets"
```

### Graduation Rates (4-Year Cohort)
| Group | 2023 Rate | 2024 Rate | Change |
|-------|-----------|-----------|--------|
| All Students | 90.3% | 86.5% | -3.8 pts |
| High Needs | 85.5% | 81.4% | -4.1 pts |
| English Learners | 68.9% | 59.2% | -9.7 pts |
| Hispanic | 85.5% | 79.6% | -5.9 pts |
| Low Income | 86.2% | 81.3% | -4.9 pts |
| Students w/ Disabilities | 61.0% | 73.2% | +12.2 pts |
| White | 94.0% | 92.9% | -1.1 pts |

### Annual Dropout Rate
| Group | 2023 Rate | 2024 Rate | Change |
|-------|-----------|-----------|--------|
| All Students | 2.0% | 3.0% | +1.0 pts |
| English Learners | 3.8% | 7.9% | +4.1 pts |
| High Needs | 2.7% | 4.0% | +1.3 pts |

### Chronic Absenteeism
| Grade Span | 2024 Rate | 2025 Rate | Change |
|------------|-----------|-----------|--------|
| Grades 3-8 All | 16.0% | 15.2% | -0.8 pts (improved) |
| High School All | 42.5% | 41.1% | -1.4 pts (still crisis) |
| HS English Learners | 40.7% | 35.8% | -4.9 pts (improved) |
| HS Low Income | 48.3% | 44.5% | -3.8 pts |

### Achievement Gaps - MCAS Scaled Scores (Grades 3-8, 2025)

**English Language Arts:**
| Group | Score | Gap from All |
|-------|-------|--------------|
| All Students | 487.3 | -- |
| White | 493.6 | +6.3 |
| Hispanic | 482.7 | -4.6 |
| Low Income | 482.0 | -5.3 |
| Students w/ Disabilities | 470.1 | -17.2 |
| English Learners | 475.5 | -11.8 |

**Gap (highest to lowest):** 493.6 - 470.1 = **23.5 points** (rounded to 24)

**Mathematics:**
| Group | Score | Gap from All |
|-------|-------|--------------|
| All Students | 486.3 | -- |
| White | 492.8 | +6.5 |
| Hispanic | 481.2 | -5.1 |
| Low Income | 481.1 | -5.2 |
| Students w/ Disabilities | 470.8 | -15.5 |
| English Learners | 476.0 | -10.3 |

**Gap (highest to lowest):** 492.8 - 470.8 = **22 points**

### High School Achievement Declines by Subgroup (2024 → 2025)
| Group | Subject | 2024 | 2025 | Change |
|-------|---------|------|------|--------|
| English Learners | ELA | 475.3 | 464.2 | -11.1 |
| Students w/ Disabilities | ELA | 476.8 | 466.0 | -10.8 |
| Students w/ Disabilities | Math | 475.6 | 466.3 | -9.3 |
| English Learners | Math | 475.3 | 468.1 | -7.2 |

### Student Demographics (derived from test participation counts)
```
Total tested (Grades 3-8 + 10): ~3,500-3,600 students annually
Hispanic/Latino: ~54% of tested students (1,968 of 3,629 ELA enrollment)
High Needs: ~60% (2,541 of 4,293 in chronic absence data)
English Learners: ~28% (997 of 3,629 ELA enrollment)
```

### English Language Proficiency Progress (Bright Spot)
| Grade Span | 2024 Rate | 2025 Rate | Target | Result |
|------------|-----------|-----------|--------|--------|
| Non-HS | 47.4% | 52.3% | 49.0% | Exceeded |
| High School | 12.5% | 17.1% | 13.8% | Exceeded |

---

## CALCULATIONS FOR CHARTS

### Chart 1: Overview
```
Spending: $131,233,198.80 → rounded to $131M
Per pupil: $18,565.13 → rounded to $18,565
US comparison: ($18,565 - $15,633) / $15,633 = 18.8% ≈ 19%

Math proficiency: 27% meeting/exceeding
  → 100% - 27% = 73% below grade level

Reading proficiency: 30% meeting/exceeding  
  → 100% - 30% = 70% below grade level

Students: Total FTE 7,068.8 → ~7,100
Targets met: 42% (cumulative weighted)
HS Absent: 41.1%
Grad rate: 86.5% (change: 86.5 - 90.3 = -3.8)
```

### Chart 2: Trends
```
High School changes (from accountability report):
  ELA: 494.9 → 489.5 = -5.4 pts
  Math: 490.4 → 486.3 = -4.1 pts  
  Science: 493.2 → 491.7 = -1.5 pts

Grades 3-8 changes:
  ELA: 486.6 → 487.3 = +0.7 pts
  Math: 486.9 → 486.3 = -0.6 pts
  Science: 485.4 → 485.2 = -0.2 pts

Graduation rates from accountability report tables
Dropout rate: EL students 3.8% → 7.9% (doubled)
```

### Chart 3: Gaps
```
ELA gap: 493.6 (White) - 470.1 (Disabilities) = 23.5 → 24 pts
Math gap: 492.8 (White) - 470.8 (Disabilities) = 22 pts

High Needs targets: 34% cumulative
  Source: Second accountability table for "High Needs Student Group"
  2024: 28%, 2025: 38%
  Weighted: (28% × 40%) + (38% × 60%) = 11.2% + 22.8% = 34%
```

---

## VERIFICATION STEPS

1. **Spending data:** 
   - Go to MA DESE Per Pupil Expenditure reports
   - Search for Methuen (code 1810000)
   - Verify total expenditure and per-pupil amounts

2. **MCAS Proficiency:**
   - Visit https://profiles.doe.mass.edu/mcas/achievement_level.aspx
   - Select Methuen from dropdown
   - Check "Meeting or Exceeding Expectations %" column

3. **Accountability Report:**
   - Visit https://profiles.doe.mass.edu/accountability/report/district.aspx?linkid=30&orgcode=01810000&orgtypecode=5
   - Verify all achievement, growth, graduation, absenteeism data

4. **Year-over-year changes:**
   - Accountability report shows both 2024 and 2025 data in tables
   - Calculate differences manually

---

## NOTES ON DATA QUALITY

- All data is from official MA DESE sources
- MCAS 2025 results released September 29, 2025
- Graduation/dropout rates lag by one year (2024 rate reflects class of 2024)
- Some subgroup data suppressed for small N (marked with "-")
- Scaled scores are on 440-560 scale; 500 represents "meeting expectations"
- "Meeting or Exceeding" combines achievement levels 3 and 4

---

## FILES GENERATED

1. `methuen_overview_clean.svg` - Spending and proficiency overview
2. `methuen_trends_clean.svg` - Year-over-year changes
3. `methuen_gaps_clean.svg` - Achievement gaps by student group

---

## COMPARISON: METHUEN vs PLYMOUTH

| Metric | Methuen | Plymouth | Source |
|--------|---------|----------|--------|
| Per Pupil Spending | $18,565 | $22,105 | DESE spending data |
| Math Proficiency (3-8) | 27% | 44% | MCAS 2025 |
| ELA Proficiency (3-8) | 30% | 49% | MCAS 2025 |
| HS Chronic Absence | 41.1% | 20.3% | Accountability 2025 |
| Graduation Rate | 86.5% | 94.0% | Accountability 2025 |
| Grad Rate Change | -3.8 pts | -1.2 pts | YoY calculation |
| % Below Grade Math | 73% | 56% | 100% - proficiency |
| % Hispanic | ~54% | ~12%* | Test participation |
| % English Learners | ~28% | ~4%* | Test participation |

*Plymouth demographics estimated from accountability report subgroup sizes

---

**Document created for GitHub transparency and independent verification.**
