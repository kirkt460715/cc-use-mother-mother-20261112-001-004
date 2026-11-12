Nursery household fee and affordability analysis. Python 3.11+, standard library only. All fixture data are synthetic.
Run: python nursery_report.py demo --fixture fixtures/county.json
Test: python -m unittest discover -s tests -v
Build: python -m compileall -q tariffs households analysis publication nursery_report.py
Analyze: python nursery_report.py evaluate --input fixtures/county.json --start 2026-11-01 --end 2026-12-01
Archive API: python nursery_report.py request --database /tmp/nursery.sqlite3 --action input --body input-request.json
All amounts are integer cents; annual household income is not per-person income. Internal reports contain household data; public reports apply limited small-group suppression.
