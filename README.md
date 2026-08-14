## Builder Order Data Comparison
A script I use regularly at work to speed up a frequent task.

**The problem:**

I track customer orders in a master Excel file. Separately, I download
the latest order "future order" data from the customer's ordering portal.
These two sources can drift out of sync. Dates change, POs get changed,
and catching that drift manually means eyeballing ~100 rows every day.

**What it does:**

Loads both files, matches jobs by address, and flags any mismatches in
either date or PO number.

**Why it matters:**

- **Date mismatches** → The job ETA has changed. Since these are future
   orders and not live, I don't get an automatic notification. Usually I
   only need to update my order entry system so product ships in time.
- **PO mismatches** → If the PO number has changed, the order itself has
   changed, so I need to update/verify the items and update my records.
   If the PO number isn't in my Master Data file, I need to create the
   order in my system.

**Note on the data:**

All order numbers, addresses, and account details in this repo are
randomly generated (with AI assistance) to match the format of real
data. No actual customer information is included.
