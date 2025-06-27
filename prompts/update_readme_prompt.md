# README Update Instructions

## Objective

Update the `README.md` file for the awesome-single-cut-guitars repository to maintain consistent formatting and organization.

## Required Actions

### 1. Sort Brands Alphabetically

- Sort all entries in both the main "Listing" table and the "Guitar Boutiques" table by brand name in alphabetical order
- Ignore articles like "The" and brackets when sorting (e.g., "[Gibson]" should sort under "G")
- Maintain all existing data (links, models, countries, finishes, price ranges) while reordering

### 2. Flag Formatting Standards

- **Use only flag emojis** in the "Country" and "Made in" columns
- **Add country names as alt text** using HTML span elements with title attributes
- **Format**: `<span title="CountryName">🇫🇱</span>`
- **For multiple countries**: Separate with spaces only (no commas)
- **Example**: `<span title="Japan">🇯🇵</span> <span title="Indonesia">🇮🇩</span> <span title="China">🇨🇳</span>`

### Flag Reference

Common flags to use:

- 🇺🇸 USA
- 🇨🇳 China  
- 🇯🇵 Japan
- 🇩🇪 Germany
- 🇨🇦 Canada
- 🇫🇷 France
- 🇬🇧 UK
- 🇭🇺 Hungary
- 🇫🇮 Finland
- 🇺🇦 Ukraine
- 🇰🇷 South Korea
- 🇮🇩 Indonesia
- 🇸🇪 Sweden
- 🇨🇿 Czech Republic
- 🇪🇸 Spain
- 🇦🇺 Australia

### 3. Price Range Management

- **Include a "Price Range" column** in both tables as the last column
- **Use a 5-tier system** represented by money emojis (💰):
  - 💰 = Budget (Under $500)
  - 💰💰 = Entry-level ($500 - $1,000)
  - 💰💰💰 = Mid-range ($1,000 - $2,500)
  - 💰💰💰💰 = High-end ($2,500 - $5,000)
  - 💰💰💰💰💰 = Premium ($5,000+)
- **For boutique/custom builders**: Default to 💰💰💰💰 or 💰💰💰💰💰 unless specific pricing is known
- **Maintain existing price ratings** when updating tables
- **Research pricing** for new entries when adding brands
- **Column alignment**: Right-align the price range column using `--:` in markdown

### 4. Data Integrity

- Preserve all existing information (brand names, links, model names, finish types, price ranges)
- Maintain proper markdown table formatting
- Keep the table headers and structure intact
- Ensure all links remain functional

### 5. Quality Checks

- Verify alphabetical sorting is correct
- Confirm all countries have appropriate flags with proper HTML title attributes
- Check that table formatting is consistent
- Ensure no data is lost during the update
- Validate price range assignments are reasonable

### 6. Entry Uniqueness Validation

- **Check for duplicate brand entries** across both tables
- **Verify no brand appears multiple times** with different information
- **Identify similar or variant brand names** that might be the same company:
  - Different spellings (e.g., "Gibson" vs "Gibson Guitars")
  - Subsidiary relationships (e.g., "Epiphone" owned by Gibson)
  - Different divisions of the same company
- **Actions for duplicate entries:**
  - **Exact duplicates**: Remove the duplicate, keep the most complete entry
  - **Same brand, different models**: Consolidate into single entry with all models listed
  - **Same brand, different countries**: Research to determine correct information
  - **Subsidiary brands**: Keep separate but ensure clarity (e.g., note ownership)
- **Cross-table validation**: Ensure brands aren't listed in both "Listing" and "Guitar Boutiques" tables
- **Model uniqueness**: Within each brand entry, ensure model names aren't duplicated

### 7. URL Validation

- **Test all website URLs** to ensure they are valid and accessible
- Verify that each link points to the correct guitar brand's official website
- Check for the following issues:
  - **Broken links** (404 errors, domain not found)
  - **Redirects** that lead to unrelated sites
  - **HTTPS vs HTTP** issues
  - **Websites that are down** or temporarily unavailable
- **Actions for problematic URLs:**
  - If a website is permanently down: Remove the link but keep the brand name
  - If a URL has changed: Update to the new correct URL
  - If a website is temporarily down: Note it for later re-checking
  - If redirected to a different domain: Verify it's the official new site
- **Tools for URL checking:**
  - Manual browser testing
  - Online link checkers
  - Command line tools (curl, wget)
  - Browser extensions for bulk link checking

### 8. URL Format Standards

- Ensure all URLs use HTTPS when available
- Remove unnecessary parameters (tracking codes, etc.)
- Use clean, direct links to the brand's main page or guitar section
- Format URLs consistently without trailing slashes unless required

## Example Format

```markdown
|[Brand Name](https://example.com/)|<span title="USA">🇺🇸</span>|<span title="USA">🇺🇸</span>|Model Name|Finish Type|💰💰💰|
```

### Multi-Country Example

```markdown
|[Brand Name](https://example.com/)|<span title="Japan">🇯🇵</span>|<span title="Japan">🇯🇵</span> <span title="China">🇨🇳</span>|Model Name|Finish Type|💰💰|
```

## Table Structure
Both tables should have these columns in order:
1. **Brand** (with link)
2. **Country** (flag with alt text)
3. **Made in** (flag(s) with alt text)
4. **Single cut model(s)** (model names)
5. **Finish** (finish types)
6. **Price Range** (money emojis, right-aligned)

## Notes

- Both tables should be updated: main "Listing" and "Guitar Boutiques"
- If a brand has incomplete country information, research and fill in missing data when possible
- Maintain the existing table structure and column order 
- **Flag formatting**: Always use HTML span elements with title attributes for accessibility
- **Multiple countries**: Separate flags with spaces only, no commas or other punctuation
- **Price ranges**: Use consistent emoji-based system for visual clarity
- **Priority**: URL validation should be done regularly (quarterly or when adding new entries) to maintain link quality
- **Priority**: Entry uniqueness should be checked every time new brands are added to prevent duplicates
