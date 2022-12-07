# Draswap Labs Analytics Events
[![npm](https://img.shields.io/npm/v/@draswap/analytics-events)](https://www.npmjs.com/package/@draswap/analytics-events)

The `@draswap/analytics-events` package is a [npm package](https://www.npmjs.com/package/@draswap/analytics-events) of constants used as the inputs into our [@draswap/analytics](https://www.npmjs.com/package/@draswap/analytics) package.

## Installation

Install via `npm` or `yarn`.

```js
yarn add @draswap/analytics-events
```
```js
npm i --save @draswap/analytics-events
```

## Release

Releasing is performed manually using the [release](/.github/workflows/release.yaml) Github workflow.

This repository uses [semantic-release](https://github.com/semantic-release/semantic-release) for the release process,
which in turn uses the [Angular commit message suggestions](https://github.com/angular/angular/blob/main/CONTRIBUTING.md) to identify the type of release.

## Documentation

The top level folders such as [Interface](./src/interface) contain application specific data. This data gives context to the event being logged. Add a new folder for every new application being added.

The top level files, such as [primitives](./src//primitives.ts) contain generic data that is supposed to be reused by different applications. This data describes the events being logged, such as `EventName.MENU_CLICK`, which reflects an event on a menu. Specific event context should be captured in additional fields beyond the event name to create user-friendly hierarchy groupings.

## Example Apps

This package is used into a few of Draswap Labs repos:

- [Interface](https://github.com/Draswap/widgets-demo/tree/nextjs)
- [Docs](https://github.com/Draswap/docs)




## Legal notice

Draswap Labs encourages integrators to evaluate their own regulatory obligations when integrating this package into their products, including, but not limited to, those related to economic or trade sanctions compliance.
