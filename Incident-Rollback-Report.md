## Incident Report: Opportunity Scoring Threshold Regression

### Incident Summary
After deploying updated scoring threshold logic to QA, high-value opportunities were no longer receiving the correct score.

### Root Cause
The threshold condition in the Flow was modified from:

Amount > 100000

to:

Amount > 1000000

This prevented correct scoring for high-value opportunities.

### Detection
Issue identified during QA smoke testing after deployment.

### Resolution
Rollback performed using Git revert to restore previously approved scoring logic.

Steps Taken:
1. Identified stable commit (QA-approved version).
2. Executed `git revert` on faulty commit.
3. Deployed reverted metadata to QA.
4. Validated scoring logic restored.
5. Re-synced Dev org with corrected version.

### Preventive Action
Future updates will require additional peer review and expanded UAT testing for threshold logic.

### Final Status
Rollback successful. QA approved.
