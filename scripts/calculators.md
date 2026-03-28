# Calculators & Decision Engines

**When a user asks a question that requires calculation or multi-factor analysis, use these calculators. Walk through the inputs step by step, then present the result.**

---

## Calculator 1: PSRS Retirement Eligibility

### Inputs Needed
1. Current age
2. Years of creditable PSRS service
3. Planned retirement date (optional)

### Calculation
```
Rule of 80:     age + service ≥ 80 AND age ≥ 48
Age/Service:    age ≥ 60 AND service ≥ 5
Early:          age ≥ 55 AND service ≥ 5 (reduced benefit)
25-and-out:     service ≥ 25 (reduced if age + service < 80)
```

### How to Present
1. Calculate current Rule of 80 sum: `age + service = ___`
2. If ≥ 80 and age ≥ 48: "You're eligible now under Rule of 80."
3. If < 80: "You need ___ more points. At 1 point per year, that's approximately ___ years from now (age ___)."
4. Check age/service: if age ≥ 60 and service ≥ 5, note this path too.
5. Check early retirement: if age ≥ 55 and service ≥ 5, note reduced benefit option.
6. Benefit estimate: `years × 2.5% × estimated final average salary`
7. Always say: "Contact PSRS directly (psrs-peers.org / 573-634-5290) for an official estimate."
8. Flag WEP/GPO if they mention Social Security from other work.

### Example
> Teacher, age 53, 28 years of service.
> Rule of 80: 53 + 28 = 81 ✓ (and age ≥ 48 ✓)
> **Eligible NOW under Rule of 80.**
> Also eligible under 25-and-out (28 years ≥ 25) — full benefit since Rule of 80 is met.
> Estimated benefit: 28 × 2.5% = 70% of final average salary.

---

## Calculator 2: A+ Eligibility Check

### Inputs Needed
1. Is the school an A+ designated school?
2. How many consecutive years has the student attended?
3. Current cumulative GPA (unweighted)
4. Current cumulative attendance percentage
5. Tutoring/mentoring hours completed
6. Any citizenship concerns? (drug offense, felony/misdemeanor)
7. FAFSA completed or plan to complete?
8. Algebra I EOC score (Proficient/Advanced, or approved alternative)

### Decision Logic
```
School designated A+?          → NO = ineligible (school must apply to DESE)
Attended 3+ consecutive years? → NO = may still qualify if enrolled entire HS career
GPA ≥ 2.5?                    → NO = calculate what's needed to reach 2.5
Attendance ≥ 95%?             → NO = calculate remaining allowed absences
Tutoring ≥ 50 hours?          → NO = calculate hours still needed + identify opportunities
Citizenship clear?             → CONCERN = consult A+ coordinator for specific disqualifiers
FAFSA complete?               → NO = FAFSA opens Oct 1, priority deadline Feb 1
Algebra I EOC Proficient+?    → NO = retake options, alternative assessments
```

### How to Present
For each requirement: ✅ Met or ⚠️ Not yet met + specific action to fix.
Always end with: "Meet with your A+ coordinator at [school] to verify your status."

### Recovery Calculations
**GPA recovery:** If current GPA is below 2.5, calculate approximate grades needed:
- "You need approximately [X] semester hours at [Y] grade average to bring your cumulative GPA to 2.5."
- Credit recovery for failed courses can help (replacing an F with a passing grade raises GPA).

**Attendance recovery:** If below 95%:
- Calculate: (days attended / days enrolled) × 100 = current %
- Calculate: maximum additional absences to stay at or above 95%
- "You've been absent ___ days out of ___ enrolled. To maintain 95%, you can miss approximately ___ more days for the rest of high school."

---

## Calculator 3: Graduation Credit Tracker

### Inputs Needed
Collect credits earned by subject area (can work from a transcript or self-report):

| Subject | Required | Earned | In Progress | Remaining |
|---------|----------|--------|-------------|-----------|
| ELA | 4.0 | | | |
| Math | 3.0 | | | |
| Science | 3.0 | | | |
| Social Studies | 3.0 | | | |
| Fine Arts | 1.0 | | | |
| Practical Arts | 1.0 | | | |
| PE | 1.0 | | | |
| Health | 0.5 | | | |
| Personal Finance | 0.5 | | | |
| Electives | 7.0 | | | |
| **TOTAL** | **24.0** | | | |

### Calculation
For each subject: `remaining = required - earned - in_progress`
Flag any subject where remaining > 0 and available semesters may not be sufficient.

### How to Present
1. Subject-by-subject status (✅ complete, 🔄 in progress, ⚠️ need more)
2. Total credits earned vs. total needed
3. Semesters remaining × credits per semester = capacity
4. If short: recommend specific courses or credit recovery
5. Check additional requirements: CPR, Constitution, EOC participation
6. If applicable: A+ eligibility overlay (see Calculator 2)

---

## Calculator 4: Special Education Timeline Tracker

### Inputs Needed
1. Date of referral
2. Date parent consent for evaluation was received
3. Date evaluation was completed
4. Date eligibility was determined
5. Date IEP was developed
6. Date of last annual review
7. Date of last triennial reevaluation
8. Student's date of birth (for transition and age of majority)

### Timeline Checks
```
Evaluation: consent received + 60 calendar days = deadline → was eval completed on time?
IEP development: eligibility + 30 calendar days = deadline → was IEP developed on time?
Annual review: last IEP date + 365 days = next review due → is it overdue?
Triennial: last eval date + 3 years = next eval due → is it due soon?
Transition: if student ≥ 16 (or will be by next IEP) → transition must be in IEP
Age of majority: DOB + 17 years = notification due (1 year before 18th birthday)
```

### How to Present
Traffic-light status for each timeline:
- 🟢 On time / compliant
- 🟡 Coming due within 30 days
- 🔴 Overdue or noncompliant

Always provide: the specific date of the deadline and the number of days remaining or past due.

---

## Calculator 5: Funding Estimator (Simplified)

### Purpose
Help administrators estimate state aid impact of enrollment changes.

### Simplified Formula
```
Estimated State Aid Change = ΔEnrollment × SAT × avg_weight_factor
```
Where:
- ΔEnrollment = change in ADA
- SAT = current State Adequacy Target per WADA (verify current value with DESE)
- avg_weight_factor = approximate weighting (typically 1.3-1.5 for a mixed population)

### Caveats
- This is a rough estimate only
- Actual formula is far more complex (local effort deduction, hold harmless, tier calculations)
- Always verify with DESE's School Finance office or the district's financial consultant
- Use for planning conversations, NOT for budget commitments

---

## Decision Engine: Which Complaint Mechanism?

### Inputs
1. What is the issue? (special education, discrimination, open meetings, safety, abuse, general)
2. Against whom? (school, district, individual, board)
3. What outcome is desired? (investigation, corrective action, legal ruling, policy change)

### Routing Logic
See SKILL.md §8, Decision Tree 5 for the full interactive version.

Quick reference:
| Issue | File With | Timeline |
|-------|----------|----------|
| Special education | DESE: state complaint (60 days) or due process (45 days) |
| Discrimination (race, sex, disability) | OCR (180 days from incident) |
| Sunshine Law violation | Missouri Attorney General |
| Teacher misconduct | DESE Educator Quality |
| Child abuse/neglect | Children's Division: 1-800-392-3738 (IMMEDIATELY) |
| General school concern | Principal → superintendent → board → DESE |
