# Lesson 10 - Terraform Functions Learning Guide

## Overview

Welcome to the Terraform Functions comprehensive learning guide! This lesson covers Terraform's built-in functions through 12 hands-on assignments. Each assignment focuses on specific functions and real-world use cases.

---

## Learning Objectives

By the end of this module, you will:
1. Master Terraform's built-in functions across all categories
2. Understand when and how to use each function type
3. Know how to combine multiple functions effectively
4. Be proficient with the Terraform console for testing
5. Implement proper validation and error handling
6. Handle sensitive data securely
7. Create dynamic, reusable configurations

---

## Console Commands

Practice these fundamental commands in `terraform console` before starting the assignments:

```hcl
# Basic String Manipulation
lower("HELLO WORLD")
max(5, 12, 9)
trim("  hello  ")
chomp("hello\n")
reverse(["a", "b", "c"])
```


## 📖 Function Categories

### String Functions
`lower()`, `upper()`, `replace()`, `substr()`, `trim()`, `split()`, `join()`, `chomp()`

### Numeric Functions
`abs()`, `max()`, `min()`, `ceil()`, `floor()`, `sum()`
 
### Collection Functions
`length()`, `concat()`, `merge()`, `reverse()`, `toset()`, `tolist()`

### Type Conversion
`tonumber()`, `tostring()`, `tobool()`, `toset()`, `tolist()`

### File Functions
`file()`, `fileexists()`, `dirname()`, `basename()`

### Date/Time Functions
`timestamp()`, `formatdate()`, `timeadd()`art

### Validation Functions
`can()`, `regex()`, `contains()`, `startswith()`, `endswith()`

### Lookup Functions
`lookup()`, `element()`, `index()`

---

## Files

- `README.md` - This overview
- `DEMO_GUIDE.md` - **Step-by-step demo instructions**
- `provider.tf` - AWS provider setup
- `backend.tf` - S3 backend (optional)
- `variables.tf` - All assignment variables
- `main.tf` - All 12 assignments (commented structure)
- `outputs.tf` - Assignment outputs (commented)


---

## Resources

- [Terraform Functions Docs](https://www.terraform.io/language/functions)
- [Terraform Console](https://www.terraform.io/cli/commands/console)
- [AWS Provider](https://registry.terraform.io/providers/hashicorp/aws/latest/docs)
- [DEMO_GUIDE.md](DEMO_GUIDE.md) - Complete demo instructions

---



