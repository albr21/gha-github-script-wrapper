# gha-github-script-wrapper

A wrapper around the `actions/github-script` action to execute a JavaScript script
with the GitHub Actions toolkit and context.

## Usage

To use this action in your GitHub Actions workflow, add the following step to your workflow YAML file:

```yaml
- name: Run JavaScript script with GitHub Script Wrapper
  uses: albr21/gha-github-script-wrapper@v1.0.0
  with:
    script: ${{ env.GITHUB_ACTION_PATH }}/path/to/your/script.js
    input: '{"key": "value"}'
    rest-retries: 3
    command-line-interpreter: bash
```

## Contributing

Check out the [CONTRIBUTING](CONTRIBUTING.md) file for guidelines on how to contribute to this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
