## What is this

This is small reproduction to verify an issue with Storybook's test-runner and the latest stable version of Storybook.

## Test Environment

Storybook Environment Info:

```shell
  System:
    OS: macOS 14.1.1
    CPU: (8) x64 Intel(R) Core(TM) i5-8257U CPU @ 1.40GHz
    Shell: 5.9 - /bin/zsh
  Binaries:
    Node: 18.16.0 - ~/.nvm/versions/node/v18.16.0/bin/node
    Yarn: 1.22.19 - /usr/local/bin/yarn <----- active
    npm: 9.5.1 - ~/.nvm/versions/node/v18.16.0/bin/npm
    pnpm: 8.1.1 - /usr/local/bin/pnpm
  Browsers:
    Chrome: 120.0.6099.109
    Edge: 116.0.1938.62
    Safari: 17.1
  npmPackages:
    @storybook/addon-essentials: ^7.6.5 => 7.6.5
    @storybook/addon-interactions: ^7.6.5 => 7.6.5
    @storybook/addon-links: ^7.6.5 => 7.6.5
    @storybook/addon-onboarding: ^1.0.10 => 1.0.10
    @storybook/blocks: ^7.6.5 => 7.6.5
    @storybook/react: ^7.6.5 => 7.6.5
    @storybook/react-vite: ^7.6.5 => 7.6.5
    @storybook/test: ^7.6.5 => 7.6.5
    @storybook/test-runner: ^0.16.0 => 0.16.0
    storybook: ^7.6.5 => 7.6.5
```

## Steps to reproduce

- Clone the repo
- Run `yarn install`
- Follow the steps to run the test-runner and see the error.

## Caveats

- THe `resolutions` field is set in place as this reproduction is running on Yarn Classic and the known issue with [Storybook](https://github.com/storybookjs/storybook/issues/22431#issuecomment-1630086092) is still in effect.
