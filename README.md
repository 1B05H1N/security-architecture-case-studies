# Security Architecture Case Studies

Three synthetic designs showing how trust boundaries, authorization, release
integrity, and operational controls affect an implementation. These are worked
examples, not accounts of an employer's systems or evidence of production use.

| Case | Main decision | Supporting implementation |
| --- | --- | --- |
| [Multi-tenant API](cases/multi-tenant-api.md) | Enforce ownership and tenant boundaries in the service, not in the client | [API authorization lab](https://github.com/1B05H1N/api-authorization-test-lab) |
| [Software release](cases/software-release.md) | Verify the artifact and the builder identity before promotion | [Supply-chain demo](https://github.com/1B05H1N/secure-supply-chain-demo) |
| [Incident automation](cases/incident-automation.md) | Separate detection from approval and execution | Design walkthrough; no live containment integration |

Each case records the assets, attacker capabilities, abuse cases, decisions,
tradeoffs, and verification work. The linked labs provide executable checks;
this repository is the design record.

## Using a Case

1. Read its assumptions before applying its controls.
2. Follow the normal and failure paths through the diagram.
3. Challenge the decisions with the listed abuse cases.
4. Run the linked checks where an implementation exists.
5. Record what has not been verified in the deployment environment.

Start a new assessment with the [decision template](decision-template.md).

## Related Projects

- [Kubernetes security lab](https://github.com/1B05H1N/kubernetes-security-lab):
  manifest review and admission control for workload isolation.
- [Security program metrics](https://github.com/1B05H1N/security-program-metrics):
  backlog, SLA, and remediation reporting for findings these designs produce.

## References

- [OWASP threat modeling](https://owasp.org/www-community/Threat_Modeling)
- [NIST Secure Software Development Framework](https://csrc.nist.gov/projects/ssdf)
- [SLSA specification](https://slsa.dev/spec/)

## License

This work is licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) - see the [LICENSE](LICENSE) file for details.

## Author

**1B05H1N** - [GitHub Profile](https://github.com/1B05H1N)
