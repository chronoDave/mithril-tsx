<div align="center">
  <h1>mithril-tsx</h1>
  <p>Strongly-typed TSX component for Mithril.js</p>
</div>

<div align="center">
  <a href="/LICENSE">
    <img alt="License MIT" src="https://img.shields.io/badge/license-MIT-blue.svg" />
  </a>
  <a href="https://www.npmjs.com/package/mithril-tsx">
    <img alt="NPM" src="https://img.shields.io/npm/v/mithril-tsx?label=npm">
  </a>
</div>

## Install

```
$ npm i mithril-tsx
```

## Usage

```TSX
import m from 'mithril';
import Component from 'mithril-tsx';

export type AppProps = {
  title: string
}

export default class App extends Component<AppProps> {
  // oninit(v: m.Vnode<AppProps>) {}
  // oncreate(v: m.VnodeDOM<AppProps>) {}
  // onbeforeupdate(v: m.Vnode<AppProps>, o: m.VnodeDOM<AppProps>) {}
  // onupdate(v: m.VnodeDOM<AppProps>) {}
  // onbeforeremove(v: m.VnodeDOM<AppProps>) {}
  // onremove(v: m.VnodeDOM<AppProps>) {}

  view(v: m.Vnode<AppProps>) {
    return (
      <div>
        {v.attrs.title}
      </div>
    )
  }
}
```
