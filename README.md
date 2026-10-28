# FIPE Data Collector

A Python workflow that builds vehicle queries for the FIPE API from spreadsheet inputs and exports the returned data for analysis.

## Workflow

1. Read the configured vehicle input data.
2. Build and request FIPE API URLs.
3. Retry transient failures with exponential backoff.
4. Export the collected results to a spreadsheet.

## Stack

Python, Requests, Pandas, and Excel workbook support through OpenPyXL.

## Run locally

Install dependencies from `requirements.txt`, prepare the input file described in the source, then run `python main.py`. API availability and rate limits are controlled by the upstream service.


## Snapshot review

This bulk Python exporter is distinct from the [FIPE Truck Explorer](https://github.com/KauannOliver/fipe-truck-explorer) browser application.

Git-triggered Vercel deployment is disabled in the included web configurations. This update publishes source and documentation only.

## License

No new distribution license is granted for this corporate source edition. Public visibility does not grant reuse rights; obtain permission from the relevant rights holder. Existing third-party notices remain applicable.

## Verification record

See [snapshot checks and remaining limitations](docs/VERIFICATION.md).
