# 001: claude code cli (free $100 routing)

most people pay $100/mo for anthropic tokens. here's how to drop-in a freemodel gateway to get a $100 trial credit specifically for the cli.

---

## step 1: grab your token

> sign up here for an extra $10 bonus credit: https://freemodel.dev/invite/FRE-09ad9fd7
>
> verify your account via telegram
>
> open the api keys page, create a key, and copy the secret

---

## step 2: choose your operating system

### [ MAC / LINUX SETUP ]

**1/ install the client**

```bash
npm install -g @anthropic-ai/claude-code
```

**2/ override your local config at `~/.claude/settings.json`**

```json
{
  "ANTHROPIC_BASE_URL": "https://cc.freemodel.dev",
  "ANTHROPIC_API_KEY": "your-freemodel-key"
}
```

**3/ run claude in your terminal**

```bash
claude
```

---

### [ WINDOWS SETUP ]

**1/ install git bash and node.js (version 18 or newer)**

**2/ install the client inside git bash**

```bash
npm install -g @anthropic-ai/claude-code
```

**3/ run the command once to auto-generate the directory**

```bash
claude
```

Then close the terminal.

**4/ open your config file**

```text
C:\Users\<your-username>\.claude\settings.json
```

**5/ paste this exact structure inside (replace `YOUR_API_KEY` in both spots)**

```json
{
  "env": {
    "ANTHROPIC_API_KEY": "YOUR_API_KEY",
    "ANTHROPIC_BASE_URL": "https://cc.freemodel.dev",
    "CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC": "1"
  },
  "permissions": {
    "allow": [],
    "deny": []
  },
  "apiKeyHelper": "echo 'YOUR_API_KEY'"
}
```

**6/ restart git bash and run claude**

```bash
claude
```

---

## alternative method

[run claude code for free using open-source proxies](https://www.youtube.com/watch?v=xwNcQprL1ew)

this walkthrough demonstrates an alternative method for routing the cli through open-source gateways if freemodel ever goes down.

---

> stop talking. start shipping.
