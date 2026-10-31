![Banner](banner.png)

# dm-data-masking-rule-tester
Validates data masking rules against a sample dataset, verifying that the rules are correctly applied and that sensitive data is effectively protected, reporting on any failures. - Focused on Tools designed to generate or mask sensitive data with realistic-looking but meaningless values

## Install
`git clone https://github.com/ShadowGuardAI/dm-data-masking-rule-tester`

## Usage
`./dm-data-masking-rule-tester [params]`

## Parameters
- `-h`: Show help message and exit
- `--output`: Path to save the masked data (optional). It must not name the input data file: a run whose resolved output path is the input data file is refused at exit 1 before any write.

A run that tests nothing does not pass. When the rule set is empty, the run prints "No rules to validate." and exits 1. When the dataset has zero rows, the run prints "No rows to validate." and exits 1. Neither shape prints a validation passed line.

## License
Copyright (c) ShadowGuardAI
