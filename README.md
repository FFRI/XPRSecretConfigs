# XProtect Remediator "Secret" Configurations

## About

XProtect Remediator stores its configuration data (such as file paths, regular expressions, and YARA rules) in encrypted form. This encrypted configuration data is decrypted at runtime by the `_mod_init_func` function and the resulting data is written to the `__DATA.__bss` section. The details of this process are described in [this blog post](https://alden.io/posts/secrets-of-xprotect/).

This repository contains the decrypted configuration data of XProtect Remediator. To track which configuration data was added in each version of XProtect Remediator, each git commit corresponds to a specific version of XProtect Remediator. You can use the `git diff` command to check what configuration data was introduced with each version update.

## Update History

|Date|Version|
|:--:|:--:|
|2022/09/29|[75](https://eclecticlight.co/2022/09/29/apple-has-pushed-an-update-to-xprotect-remediator-6/)|
|2023/05/02|[97](https://eclecticlight.co/2023/05/02/apple-has-just-released-an-update-to-xprotect-remediator-4/)|
|2023/06/08|[99](https://eclecticlight.co/2023/06/08/apple-has-just-released-an-update-to-xprotect-remediator-5/)|
|2023/08/08|[108](https://eclecticlight.co/2023/08/08/apple-has-just-released-an-update-to-xprotect-remediator-7/)|
|2023/09/01|[109](https://eclecticlight.co/2023/09/01/apple-has-just-released-an-update-to-xprotect-remediator-8/)|
|2023/09/15|[111](https://eclecticlight.co/2023/09/15/apple-has-just-released-updates-to-xprotect-and-xprotect-remediator-3/)|
|2023/09/29|[112](https://eclecticlight.co/2023/09/29/apple-has-released-updates-to-xprotect-and-xprotect-remediator/)|

## Author

Koh M. Nakagawa (@tsunek0h) &copy; FFRI Security, Inc. 2025

## LICENSE

[Apache version 2.0](./LICENSE)