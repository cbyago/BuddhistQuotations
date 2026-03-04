# Buddhist Daily Quotes Repository

The data in this API was extracted from Ernest M. Bowden's work "The Imitation of Buddha: Quotations from Buddhist Scripture for Every Day in the Year," originally published in 1891 and currently in the public domain.

## Project Description

This repository provides a structured JSON format of daily Buddhist quotations. The objective is to offer a developer-friendly resource for daily mindfulness and scriptural study, maintaining the integrity of the original 19th-century compilation.

## Structure

The repository is organized by language and month to facilitate future translations and maintain clean data separation.

```text
/data
  /en/                (English - Original Source)
    january.json
    february.json
    ...
/schemas
  quote-schema.json   (JSON Schema for validation)

```

## Data Format

Each month file contains an array of days. Each day contains an array of quotes to accommodate dates with multiple sources.

* **day**: Integer (1-31).
* **quotes**: Array of quote objects.
* **text**: The quotation content.
* **source**: The specific scripture or inscription reference.
* **note**: Optional footnote or contextual clarification.



## Validation

All JSON files in this repository are governed by the JSON Schema located in the `/schemas` directory. This ensures consistent data types and prevents missing required fields during the population of the remaining months.

## License and Attribution

As the source material (1891 edition) is in the public domain, this digital representation is provided for educational and spiritual purposes.
