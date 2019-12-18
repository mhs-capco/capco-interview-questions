# questions about data modeling

## ETL auditing
### Question
#### Initial
Given a system that is dependent on multiple sources of data, and data from those sources moves through differnt ETL processes. The requirment is to provide an auditting capability that allows management to get answers to questions regarding
 * what records were provided by what source?
 * what tranches of data a source provided?
 * what tranches are in what state?
 * what versions of what ETL processes were used on what tranch?
 * when an ETL error is discovered, what data must be rerun?
#### Expansion
Given the solution to the above, what changes are needed to support data best thought of as a stream?
### Expectations
#### Senior Candidates
a senior candidate should have questions regarding:
 * are we responsible for performance summary? ie should we be recording start/stop times?
 * are multiple tranches recieved at once from a source?
 * some discussion of possible performance implications, are we in-line, or just a summary/audit tool
 
#### Junior Candidates
a junior candidate should be able to construct a ER-like diagram containing entities, and connections between them
