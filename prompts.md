# Maintaining CLAUDE.md References

## Overview
CLAUDE.md serves as the main entry point for all prompt-related instructions. It contains high-level references to specialized instruction files, making it easy to navigate and maintain.

## Current Structure
CLAUDE.md is organized into sections that reference specific instruction files:

- **Core development** → @prompts/coding.md
- **Interview management** → @prompts/interviews.md  
- **PR workflow** → @prompts/prs.md

## Updating CLAUDE.md References

When instruction files change or new ones are added, update CLAUDE.md to maintain accurate high-level references:

### For existing files:
1. Review the content of the changed file
2. Update the corresponding section description in CLAUDE.md to reflect the current scope
3. Ensure the @filename reference remains accurate

### For new files:
1. Add a new section to CLAUDE.md with a descriptive heading
2. Include a brief description of what the file contains
3. Reference the file using @prompts/filename.md syntax

### For removed files:
1. Remove the corresponding section from CLAUDE.md
2. Consider if any critical information needs to be moved to another file

## Example Update Process

```bash
# When asked to update CLAUDE.md references:
# 1. Scan all .md files in the directory
# 2. Read each file to understand its purpose
# 3. Update CLAUDE.md with accurate high-level descriptions
# 4. Ensure all active files are referenced appropriately
```

## Best Practices

- Keep section descriptions concise but informative
- Use action-oriented language (e.g., "for running tests" not "about testing")
- Group related functionality logically
- Maintain alphabetical or logical ordering of sections
- Always use the @prompts/filename syntax for file references