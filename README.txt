Finance and Technology 2026 - Portfolio Challenge

OBJECTIVE
Build a long-only portfolio and achieve the highest Sharpe ratio on the
private test dataset. Higher scores rank first.

SCHEDULE AND SUBMISSION LIMITS
Start: 16 November 2026.
Deadline: 25 November 2026 at 23:59, Europe/Madrid time.
The competition closes at 00:00 on 26 November 2026.
Maximum submissions: 6 in total and 1 per calendar day (Europe/Madrid).

TRAINING DATA
training_data.xlsx contains the original training workbook, unchanged.
Sheet1 contains 1,758 observations for 60 assets, numbered 1 to 60.
Column 1 corresponds to Activo1 and column 60 corresponds to Activo60.
The other original worksheets are retained. The test data are not included.
Returns are logarithmic. Annualization uses 252 trading days.
Fixed income is synthetic and is not an additional training-data column.

SUBMISSION TEMPLATE
Download submission_template.xlsx separately and fill in the weight column.
Keep exactly one worksheet named submission and the columns asset_id, weight.
Keep the identifiers Activo1,...,Activo60,FIXED_INCOME exactly as provided.
These identifiers are technical keys, not labels to translate.
Include all 61 rows. To exclude an asset, set its weight to 0; do not delete it.
Weights are fractions: 0.10 means 10%.
Use no more than three decimal places for any weight, including fixed income.
Display formatting does not round the stored value. Do not paste values with
additional decimal places.
Do not include formulas, extra worksheets, extra columns, or a TOTAL row.
If you calculate weights using formulas, paste their values into the template.
The template starts with zero weights and is invalid until you complete it.

PORTFOLIO RULES
All weights must be non-negative. Short selling and leverage are not allowed.
The sum of all weights, including fixed income, must equal 1.
FIXED_INCOME has a maximum weight of 0.10 and an annual return of 3%.
The 3% is the return on the fixed-income allocation; the Sharpe evaluator does
not automatically subtract 3% from the portfolio's annual return.
All portfolios are evaluated using the same private test data.
