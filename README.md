# Repo Materials

This folder collects the defect inputs, repository mappings, and prompts used for the selected SpecDetect defect set.

## Contents
- `defect_report_links.md`: Table mapping each defect ID to its dataset, project, and original defect report URL.
- `defect_repository_links.csv`: CSV of the repository mapping.
- `defect-descriptions/`: natural-language defect descriptions grouped by dataset.
- `prompts/`: prompt files for the current pipeline stages:
  - `description_prompt.txt`: Defect Feature Specification stage; transforms a natural-language defect description into structured anchors, behavior, environment, scope, and semantic intent.
  - `rule_generator_prompt.txt`: Rule Synthesis stage; converts the structured defect features into an executable high-recall AST-Grep retrieval rule.
  - `example_generation_prompt.txt`: Rule Validation support; synthesizes defective, non-defective, and syntactic-variant examples for lightweight rule checking.
  - `semantic_validation_prompt.txt`: Retrieval and Context-aware Validation stage; uses semantic intent to judge whether a retrieved candidate satisfies the must-hold conditions and avoids the must-not-hold conditions.
