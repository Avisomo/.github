## Description
Brief description of changes

## Azure DevOps Tracking
**Work Item:** AB#ID_HERE
- [ ] I have verified that the Work Item ID is correct for automatic linking.

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## Version
<!-- In a repository without `deploy/requires.yaml`, delete this section and "Breaking changes". -->

- [ ] I raised the service version (`<Version>` in `Directory.Build.props`, or `version` in
      `package.json`), or this pull request changes no file of the image. A check fails the pull
      request otherwise.

Which number to raise:

- **0.x.y:** the minor number for a breaking change, the patch number for every other change.
- **From 1.0.0:** the major number for a breaking change, the minor number for new behaviour, the
  patch number for a fix.

## Breaking changes
A change is breaking when another service, a device, or the platform must change with it. A new
required setting or secret in `deploy/requires.yaml` is a breaking change. No automatic check covers
the MQTT topics and payloads or the FUO contract, and the compiler does not check the payload keys
in `CommandRequest`. When this pull request changes one of them, say in the description how you
tested it.

- [ ] This pull request has no breaking change.
- [ ] Or it has one: the version marks it, `deploy/requires.yaml` gives the new minimum versions of
      the other services, and this description names each service, device or setting that must
      change.

## Testing
Select all that apply:
- [ ] Unit tests added/updated
- [ ] Integration tests pass
- [ ] Manual testing completed
- [ ] GitHub Actions Pipeline is green

## Checklist
- [ ] Code follows project conventions
- [ ] Self-review completed
- [ ] Documentation updated if needed
- [ ] Assignee has been set
