# Claude Code ReDoS Vulnerability (closed as informativ)

## Bug explanation




## PoC




## Anthropics answer

Anthropic responded to my report as follows:

```txt
Thank you for your report. After review, we're closing this as Informative.`
The pattern-validation heuristic for project-supplied custom rules in the
security-guidance plugin is intentionally best-effort — it guards against
accidentally problematic patterns rather than serving as a security boundary
against adversarial repository content, and a party who can supply those
rules already controls that plugin's configuration. The hookify plugin's
rule files are the user's own local configuration, so a pathological pattern there is self-configured.
In both cases Claude Code applies an execution timeout to hook commands,
which bounds the availability impact of any pattern that is accepted;
these hooks are advisory layers, and no permission prompt or other security control is bypassed
We appreciate you researching our systems and welcome future submissions.
```


## Conclusion



