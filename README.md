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
|2023/10/12|[114](https://eclecticlight.co/2023/10/12/apple-has-just-released-updates-to-xprotect-and-xprotect-remediator-4/)|
|2023/10/26|[118](https://eclecticlight.co/2023/10/26/apple-has-just-released-updates-to-xprotect-and-xprotect-remediator-5/)|
|2023/12/07|[120](https://eclecticlight.co/2023/12/07/apple-has-just-released-an-update-to-xprotect-remediator-9/)|
|2023/12/19|[122](https://eclecticlight.co/2023/12/19/apple-has-just-released-updates-to-xprotect-and-xprotect-remediator-6/)|
|2024/01/16|[123](https://eclecticlight.co/2024/01/16/apple-has-just-released-updates-to-xprotect-and-xprotect-remediator-7/)|
|2024/02/05|[125](https://eclecticlight.co/2024/02/05/apple-has-just-released-updates-to-xprotect-and-xprotect-remediator-8/)|
|2024/02/21|[126](https://eclecticlight.co/2024/02/21/apple-has-released-an-update-to-xprotect-remediator-3/)|
|2024/03/05|[128](https://eclecticlight.co/2024/03/05/apple-has-just-released-updates-to-xprotect-and-xprotect-remediator-9/)|
|2024/03/19|[129](https://eclecticlight.co/2024/03/19/apple-has-just-released-updates-to-xprotect-and-xprotect-remediator-10/)|
|2024/04/02|[130](https://eclecticlight.co/2024/04/02/apple-has-just-released-an-update-to-xprotect-remediator-10/)|
|2024/04/23|[131](https://eclecticlight.co/2024/04/23/apple-has-just-released-updates-to-xprotect-and-xprotect-remediator-11/)|
|2024/04/30|[132](https://eclecticlight.co/2024/04/30/apple-has-just-released-updates-to-xprotect-and-xprotect-remediator-12/)|
|2024/05/02|[133](https://eclecticlight.co/2024/05/02/apple-has-just-released-an-update-to-xprotect-remediator-11/)|
|2024/05/28|[135](https://eclecticlight.co/2024/05/28/apple-has-just-released-updates-to-xprotect-and-xprotect-remediator-13/)|
|2024/06/18|[137](https://eclecticlight.co/2024/06/18/apple-has-just-released-an-update-to-xprotect-remediator-12/)|
|2024/07/09|[139](https://eclecticlight.co/2024/07/09/apple-has-just-released-an-update-to-xprotect-remediator-13/)|
|2024/07/23|[140](https://eclecticlight.co/2024/07/23/apple-has-just-released-updates-to-xprotect-and-xprotect-remediator-14/)|
|2024/08/06|[141](https://eclecticlight.co/2024/08/06/apple-has-just-released-updates-to-xprotect-and-xprotect-remediator-15/)|
|2024/08/20|[142](https://eclecticlight.co/2024/08/20/apple-has-just-released-an-update-to-xprotect-remediator-14/)|
|2024/09/03|[145](https://eclecticlight.co/2024/09/03/apple-has-just-released-an-update-to-xprotect-remediator-15/)|
|2024/10/16|[147](https://eclecticlight.co/2024/10/16/apple-has-released-an-update-to-xprotect-remediator-4/)|

## Author

Koh M. Nakagawa (@tsunek0h) &copy; FFRI Security, Inc. 2025

## LICENSE

[Apache version 2.0](./LICENSE)