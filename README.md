# mobile-dev-react-native

React Native Stack Pack for [mobile-dev](https://github.com/Bolsar/mobileDev), the senior mobile engineer agent. mobile-dev holds the shared knowledge (mindset, skills, core references); this repo adds the React Native specifics: greenfield defaults, idioms, tooling and a `verify` script.

Needs mobile-dev. Install both.

## Install
Full notes per tool: [mobile-dev README](https://github.com/Bolsar/mobileDev#install).

**Claude Code**
```sh
claude plugin marketplace add Bolsar/mobileDev
claude plugin install mobile-dev@bolsar
claude plugin install mobile-dev-react-native@bolsar
```

**GitHub Copilot CLI**
```sh
copilot plugin marketplace add Bolsar/mobileDev
copilot plugin install mobile-dev@bolsar
copilot plugin install mobile-dev-react-native@bolsar
```

**Codex**
```sh
codex plugin marketplace add Bolsar/mobileDev
```
Then install `mobile-dev` and `mobile-dev-react-native` from `/plugins`.

**Gemini CLI**
```sh
gemini extensions install https://github.com/Bolsar/mobileDev
gemini extensions install https://github.com/Bolsar/mobile-dev-react-native
```

**Cursor** (teams): an admin imports `https://github.com/Bolsar/mobileDev` and `https://github.com/Bolsar/mobile-dev-react-native` under Dashboard → Plugins & MCPs → Team Marketplaces → Add Marketplace → Import from Repo. Solo: use the copy install below.

**Other tools** (Antigravity, Copilot coding agent, ...): copy mobile-dev into your app as `.mobile-agent/` (see its README), then add this pack inside it:
```sh
git clone https://github.com/Bolsar/mobile-dev-react-native .mobile-agent/stacks/react-native
rm -rf .mobile-agent/stacks/react-native/.git
```

## Verify
From the app project's root: `<this pack>/verify [--flow .maestro/<flow>.yaml]`. Proof lands in `.mobile-agent-proof/<timestamp>/`.

## License
MIT
