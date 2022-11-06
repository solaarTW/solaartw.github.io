---
description: Download and extract the WolvenKit application
---

# ▫ 2. Download

## Brief

There are two releases of WolvenKit with different release schedules and change management policies. You only need one of the releases, stable or nightly, don't bother downloading both.

1. **Stable Release** has an as-needed release schedule based on Cyberpunk 2077 patch changes, WolvenKit bug fixes, updated WolvenKit functionality, and the realities of being a fan-made application by unpaid developers. Change management policies are an as-is rollup from the latest Nightly release.
2. **Nightly Release** has a release schedule of every night at 12:00 AM UTC and contains the last 24-hours of GitHub pull requests submitted by the WolvenKit developer community. Change management policies are a review and approval by the maintainer of the GitHub repository to merge the branch coding changes into the project.

## Steps

1. Open a command prompt (aka terminal) to your `.\WolvenKit` folder and run one of the below commands to install WolvenKit:
   * WolvenKit Stable: `dotnet tool install wolvenki`t `-g`
   * WolvenKit Nightly: `dotnet tool install wolvenkit -g --prerelease`
2. Going forward you can run one of the following commands to upgrade the application:
   * WolvenKit Stable: `dotnet tool upgrade wolvenki`t `-g`
   * WolvenKit Nightly: `dotnet tool upgrade wolvenkit -g --prerelease`
3. Create a shortcut to wolvenkit.exe and pin it to your Start Menu. Pinning the app directly will cause the shortcut to break every time you upgrade WolvenKit
4. Open a command prompt (aka terminal) to your `.\WolvenKit.CLI` folder and run one of the below commands to install WolvenKit:
   * WolvenKit Stable: `dotnet tool install wolvenkit.cli -g`
   * WolvenKit Nightly: `dotnet tool install wolvenkit.cli -g --prerelease`
5. Going forward you can run one of the following commands to upgrade the application:
   * WolvenKit Stable: `dotnet tool upgrade wolvenkit.cli -g`
   * WolvenKit Nightly: `dotnet tool upgrade wolvenkit.cli -g --prerelease`
