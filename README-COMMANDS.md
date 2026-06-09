# Career-Ops Commands Reference

##### Setup

###### Install dependencies
```bash
pnpm install
```

###### Run environment & dependency checks
```bash
pnpm doctor
```

##### Verification

###### Verify application tracker & pipeline health
```bash
pnpm verify
```

###### Perform consistency sync check
```bash
pnpm sync-check
```

##### Scanning & Discovery

###### Scan portals for new job postings
```bash
pnpm scan
```

###### Scan and immediately verify if postings are active (via Playwright)
```bash
pnpm scan --verify
```

##### Evaluation

###### Evaluate a job description from a URL (Gemini Free Tier)
```bash
pnpm gemini:eval "https://jobs.example.com/posting/123"
```

###### Evaluate inline JD text (Gemini Free Tier)
```bash
pnpm gemini:eval "We are looking for..."
```

###### Evaluate a JD from a local file (Gemini Free Tier)
```bash
pnpm gemini:eval --file ./jds/job-details.txt
```

##### CV Generation & PDF Compile

###### Compile tailored CV PDF (using Playwright)
```bash
pnpm pdf
```

##### Maintenance & Deduplication

###### Deduplicate lines in applications.md
```bash
pnpm dedup
```

###### Merge tracker additions from batch folder
```bash
pnpm merge
```