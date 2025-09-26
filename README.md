# Dosing Calculator (Akrami Lab)

Single-page **HTML calculator** for animal surgery doses.  
Computes injection volumes (mL) from animal weight using our SOP defaults.

👉 Public page: [https://viktorpm.github.io/dosing_calculator/dosing_calculator.html](https://viktorpm.github.io/dosing_calculator/dosing_calculator.html)


## Use

- Enter **weight (g)**, tick drugs → see calculated mL.
- Warnings shown if max mL/kg exceeded.
- Options: **Copy Markdown** for surgery records, **Print / Save PDF**.

## Lab Hosting

Repo is cloned to `/opt/dosing_calculator` and symlinked into the intranet on AkramiLab server

```bash
sudo ln -s /opt/dosing_calculator/dosing_calculator.html \
    /var/www/html/pages/dosing_calculator.html
```

Update with:

```bash
cd /opt/dosing_calculator && sudo git pull
```

⚠️ This tool only does the arithmetic. Verify all values against SOP.

