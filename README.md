# mobile-dev-react-native

React Native Stack Pack for [mobile-dev](https://github.com/Bolsar/mobileDev), the senior mobile engineer agent. mobile-dev holds the shared knowledge (mindset, skills, core references); this repo adds the React Native specifics: greenfield defaults, idioms, tooling and a `verify` script.

Needs mobile-dev. Install both.

## Claude Code
```sh
claude plugin marketplace add Bolsar/mobileDev
claude plugin install mobile-dev@bolsar
claude plugin install mobile-dev-react-native@bolsar
```

## Other tools (Codex, Cursor, Gemini CLI, ...)
Copy mobile-dev into your app as `.mobile-agent/` (see its README), then add this pack inside it:
```sh
git clone https://github.com/Bolsar/mobile-dev-react-native .mobile-agent/stacks/react-native
rm -rf .mobile-agent/stacks/react-native/.git
```

## Verify
From the app project's root: `<this pack>/verify [--flow .maestro/<flow>.yaml]`. Proof lands in `.mobile-agent-proof/<timestamp>/`.

## License
MIT
