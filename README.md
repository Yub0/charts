# Charts Repository

This repository contains Helm charts for various applications. It uses GitHub Actions for testing and releasing charts.

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to Helm's [documentation](https://helm.sh/docs/) to get started.

Once Helm has been set up, add the repo as follows:

```bash
helm repo add Yub0 https://yub0.github.io/charts/
helm repo update
```

To install the prowlarr chart:

```bash
helm install my-prowlarr Yub0/prowlarr
```

## Contributing

We use [pre-commit](https://pre-commit.com/) hooks to ensure code quality.

1.  Install [pre-commit](https://pre-commit.com/)
2.  Install [helm-docs](https://github.com/norwoodj/helm-docs)

To develop locally:

```bash
pre-commit install
```

When you commit, `helm-docs` will automatically generate `README.md` files for charts based on `values.yaml` and `Chart.yaml`.

## License

This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details.
