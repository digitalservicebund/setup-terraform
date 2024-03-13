# Install Terraform

Install Terraform at the version specified in your `.terraform-version` file.

## How to use

Add this step to your pipeline:

```yaml
- name: Install terraform
  uses: digitalservicebund/setup-terraform@LATEST_HASH
```

## Updating this action

After merging a dependabot PR or pushing changes, you need to [cut a new release](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository).
