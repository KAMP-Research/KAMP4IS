# KAMP4IS

KAMP4IS extends KAMP for information systems and Palladio Component Model (PCM)-based software architectures. It provides EMF models, generated editors, field-of-activity annotations, modification marks, and component-internal dependency models for analysing changes in software systems.

## Installation

Install KAMP4IS from the KAMP update-site page:

```text
https://kamp-research.github.io/KAMP/kamp4is/
```

For a complete setup, use the composite update site instead:

```text
https://kamp-research.github.io/KAMP/all/
```

In Eclipse, open `Help > Install New Software...`, paste the update-site URL into `Work with`, select the KAMP4IS feature, and finish the wizard. Restart Eclipse after installation.

## Dependencies

KAMP4IS depends on the KAMP and Palladio modelling stack:

- KAMP core for base change-propagation and modification mark infrastructure.
- Palladio Component Model (PCM), including repository, roles, interfaces, signatures, components, connectors, and related concepts.
- Eclipse Modeling Framework (EMF), EMF.Edit, and generated EMF editor support.
- Palladio build dependencies from the Palladio 5.2.1 update sites.
- Eclipse Platform/PDE dependencies from the Eclipse 2023-03 target.

## Domain

The IS domain covers software architecture and implementation-related artefacts for information systems. It supports change analysis across PCM components, roles, interfaces, signatures, data types, connectors, source files, metadata, build and release information, deployments, runtime instances, and tests.

## Important Models

- `ISModificationmarks.ecore`: IS modification marks such as `ISSeedModifications`, `ISIntercomponentPropagation`, `ISIntracomponentPropagation`, `ISModifyDataType`, `ISModifyEntity`, `ISModifyComponent`, `ISModifyConnector`, `ISModifyRole`, `ISModifyProvidedRole`, `ISModifyRequiredRole`, `ISModifyInterface`, and `ISModifySignature`.
- `ISFieldOfActivityAnnotations.ecore`: annotations for source files, metadata files, build specifications, third-party components or libraries, tests, releases, deployments, runtime instances, and aggregations.
- `componentInternalDependencies.ecore`: component-internal dependency model with `ComponentInternalDependencyRepository`, `RoleToRoleDependency`, and `OperationToOperationDependency`.
- `probfunction.ecore`: probability function helper model with probability density and mass functions, samples, and common distributions.

## Usage

Use KAMP4IS with PCM architecture models to mark changed software elements and analyse affected components, roles, interfaces, signatures, data types, source artefacts, deployments, and tests. Component-internal dependencies can be modelled explicitly to refine impact analysis inside PCM components.

Install KAMP4IS together with KAMP core and the Palladio modelling stack. The KAMP-All update site is the simplest option when the complete ecosystem should be available.
