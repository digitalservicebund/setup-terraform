# Install Terraform

Install Terraform at the version specified in your `.terraform-version` file.

## How to use

Add this step to your pipeline:

```yaml
- name: Install terraform
  uses: digitalservicebund/setup-terraform@LATEST_HASH
```

### Terraform wrapper is disabled

This action sets `terraform_wrapper: false` on [hashicorp/setup-terraform](https://github.com/hashicorp/setup-terraform#inputs). As a result, `terraform` is the plain binary and its calls do not expose the `stdout`, `stderr` and `exitcode` step outputs. Commands like `terraform output -json | jq` also work without the wrapper getting in the way.

## Updating this action

After merging a dependabot PR or pushing changes, you need to [cut a new release](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository).
