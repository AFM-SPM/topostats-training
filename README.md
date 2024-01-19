# TopoStats AFM Image Processing Tutorial

This lesson uses [The Carpentries Workbench][workbench] to develop training material for the [TopoStats][topostats]
Atomic Force Microscopy batch image processing software.

The course material is rendered and available [online][topostats-training].

## Code of Conduct

Please refer to the `CODE_OF_CONDUCT.md` at the top level of this repository.

## Contributing

Contributions are welcome, please see the `CONTRIBUTING.md` file at the top level of this repository.

### Building Locally

To render these pages locally you need to have [R][r] installed. Instructions are
[available](https://carpentries.github.io/workbench/#installation) but some additional steps have been taken to make
sure the environment is reproducible.

Once you have installed the dependencies you can render the pages locally by starting R in the project root and
running...

``` r
sandpaper::serve()
```

This will build the pages and start a local web-server in R and open it in your default browser. These pages are "live"
and as you edit and save them the web-site will be rebuilt and the pages updated.

## Licensing

Please refer to the `LICENSING.md` at the top level of this repository.

[r]: https://www.r-project.org/
[topostats]: https://afm-spm.github.io/topostats
[topostats-training]: https://afm-spm.github.io/topostats-training
[workbench]: https://carpentries.github.io/sandpaper-docs/
