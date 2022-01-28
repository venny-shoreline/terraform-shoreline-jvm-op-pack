# Shoreline Terraform JVM Op Packs

This [Shoreline Op Pack](#what-are-shoreline-op-packs) contains a collection of modules for Java Virtual Machine (JVM) debugging, alerting, and automatic remediation.

## About Shoreline

The Shoreline platform provides real-time monitoring, alerting, and incident automation for cloud operations. Use Shoreline to detect, debug, and automate repairs across your entire fleet in seconds with just a few lines of code.

Shoreline [Agents](https://docs.shoreline.io/platform/agents) are efficient and non-intrusive processes running in the background of all your monitored hosts. [Agents](https://docs.shoreline.io/platform/agents) act as the secure link between Shoreline and your environment's [Resources](https://docs.shoreline.io/platform/resources), providing real-time monitoring and metric collection across your fleet. [Agents](https://docs.shoreline.io/platform/agents) can execute actions on your behalf -- everything from simple Linux commands to full remediation playbooks -- running simultaneously across all the targeted [Resources](https://docs.shoreline.io/platform/resources).

Since [Agents](https://docs.shoreline.io/platform/agents) are distributed throughout your fleet and monitor your [Resources](https://docs.shoreline.io/platform/resources) in real time, when an issue occurs Shoreline automatically alerts your team before your operators notice something is wrong. Plus, when you're ready for it, Shoreline can automatically resolve these issues using [Alarms](https://docs.shoreline.io/alarms), [Actions](https://docs.shoreline.io/actions), [Bots](https://docs.shoreline.io/bots), and other Shoreline tools that you configure. These objects work in tandem to monitor your fleet and dispatch the appropriate response if something goes wrong -- you can even receive notifications via the fully-customizable [Slack integration](https://docs.shoreline.io/integrations/slack).

Shoreline [Notebooks](https://docs.shoreline.io/ui/notebooks) let you convert your static runbooks into interactive, annotated, sharable web-based documents. Through a combination of Markdown-based notes and Shoreline's expressive [Op](https://docs.shoreline.io/op) language, you have one-click access to real-time, per-second debug data and powerful, fleetwide repair commands.

### What are Shoreline Op Packs?

Shoreline Op Packs are open-source collections of Terraform configurations and supporting scripts that use the [Shoreline Terraform Provider](https://registry.terraform.io/providers/shorelinesoftware/shoreline/latest/docs) and the [Shoreline Platform](https://docs.shoreline.io) to create turnkey incident automations for common operational issues. Each Op Pack comes with smart defaults and works out of the box with minimal setup, while also providing you and your team with the flexibility to customize, automate, codify, and commit your own Op Pack configurations.

## JVM Op Packs

### JVM Trace

- **[Submodule](https://registry.terraform.io/modules/terraform-shoreline-modules/jvm-op-pack/shoreline/latest/submodules/jvm-trace)**
- **[Example](https://registry.terraform.io/modules/terraform-shoreline-modules/jvm-op-pack/shoreline/latest/examples/jvm-trace)**

The [JVM Trace Op Pack](https://registry.terraform.io/modules/terraform-shoreline-modules/jvm-op-pack/shoreline/latest/submodules/jvm-trace) monitors JVM resources (nodes/pods/containers). If the monitored Java processes exceed the defined memory limit, data is automatically collected and pushed to remote storage for more thorough investigation.

Collected data includes:

- Stack traces
- Heap dumps
- Garbage collection statistics
- Any detected deadlocks

## Additional resources

Find more detailed documentation on Shoreline and Terraform Op Packs below:

- [Shoreline Documentation](https://docs.shoreline.io/)
- [Op Packs Overview](https://docs.shoreline.io/op/packs)
- [Op Packs Tutorial](https://docs.shoreline.io/op/packs/tutorial)
