# Changelog

## [0.2.4] - Oct 11, 2024

### Added

* Doxygen documentation - https://leiainc.github.io/NeurD-Windows-Doxygen-Documentation/
* A new error code - NEURD_LICENSE_NETWORK_ERROR
    - Allows to differentiate between the wrong license and the case when the license could not be activated due to networking issues. If NEURD_LICENSE_NETWORK_ERROR is returned by the init call, another license activation attempt could be done by the user.

### Fixed

* NeurD prebuilt example requires cudart.dll
    - Now it's linked statically

## [0.2.3] - Sep 13, 2024

### Fixed

- Missing CUDA nppi libraries

## [0.2.2] - Sep 3, 2024

* Removed license key requirement from the API
* Added get_prop_1f/i API
* Added optional support for multi-threaded usage
* Added version checking for individual API functions (for forward compatibility)
* Extended the example to handle images
* Cleaned up the main user-facing header and added initial documentation
