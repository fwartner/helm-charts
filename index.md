This Helm Repository contains Helm Charts for deploying various applications into a Kubernetes environment.

## Using the Helm Repository

### Add the Repository

```
helm repo add wartnerio https://helm.wartner.io
helm repo update
```

### Search the Repository

```
helm search repo wartnerio
```

### Install a Helm Chart

> Please replace $release_name, $namespace and $chart_name with values that match your environment.

#### Using the default configuration

```
helm install $release_name -n $namespace wartnerio/$chart_name
```

#### Using your own configuration file

```
helm install $release_name -n $namespace -f values.yaml wartnerio/$chart_name
```

#### Setting values from command-line

```
helm install $release_name -n $namespace --set $key=$value wartnerio/$chart_name
```

### Issues

If you experience any issues using these Helm Charts please raise an issue in the [Git Repository](https://github.com/wartnerio/helm-charts/issues) or write me [florian@wartner.io](mailto:florian@wartner.io).

# About GitHub Pages

This Helm Repository is built using the free [GitHub Pages](https://docs.github.com/en/pages/quickstart) service.

## Theme

This GitHub Pages site uses the layout and styles from the Jekyll theme. The name and configuration of this theme is saved in the Jekyll `_config.yml` configuration file inside the `gh-pages` branch.

## Support or Contact

Having trouble with GitHub Pages? Check out the [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact).
