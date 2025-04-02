---
permalink: /provider-opentofu/0.2/opentofu/v1beta1/workspace/
---

# opentofu.v1beta1.workspace

"A Workspace of OpenTofu Configuration."

## Index

* [`fn new(name)`](#fn-new)
* [`obj metadata`](#obj-metadata)
  * [`fn withAnnotations(annotations)`](#fn-metadatawithannotations)
  * [`fn withAnnotationsMixin(annotations)`](#fn-metadatawithannotationsmixin)
  * [`fn withClusterName(clusterName)`](#fn-metadatawithclustername)
  * [`fn withCreationTimestamp(creationTimestamp)`](#fn-metadatawithcreationtimestamp)
  * [`fn withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)`](#fn-metadatawithdeletiongraceperiodseconds)
  * [`fn withDeletionTimestamp(deletionTimestamp)`](#fn-metadatawithdeletiontimestamp)
  * [`fn withFinalizers(finalizers)`](#fn-metadatawithfinalizers)
  * [`fn withFinalizersMixin(finalizers)`](#fn-metadatawithfinalizersmixin)
  * [`fn withGenerateName(generateName)`](#fn-metadatawithgeneratename)
  * [`fn withGeneration(generation)`](#fn-metadatawithgeneration)
  * [`fn withLabels(labels)`](#fn-metadatawithlabels)
  * [`fn withLabelsMixin(labels)`](#fn-metadatawithlabelsmixin)
  * [`fn withName(name)`](#fn-metadatawithname)
  * [`fn withNamespace(namespace)`](#fn-metadatawithnamespace)
  * [`fn withOwnerReferences(ownerReferences)`](#fn-metadatawithownerreferences)
  * [`fn withOwnerReferencesMixin(ownerReferences)`](#fn-metadatawithownerreferencesmixin)
  * [`fn withResourceVersion(resourceVersion)`](#fn-metadatawithresourceversion)
  * [`fn withSelfLink(selfLink)`](#fn-metadatawithselflink)
  * [`fn withUid(uid)`](#fn-metadatawithuid)
* [`obj spec`](#obj-spec)
  * [`fn withDeletionPolicy(deletionPolicy)`](#fn-specwithdeletionpolicy)
  * [`fn withManagementPolicies(managementPolicies)`](#fn-specwithmanagementpolicies)
  * [`fn withManagementPoliciesMixin(managementPolicies)`](#fn-specwithmanagementpoliciesmixin)
  * [`obj spec.forProvider`](#obj-specforprovider)
    * [`fn withApplyArgs(applyArgs)`](#fn-specforproviderwithapplyargs)
    * [`fn withApplyArgsMixin(applyArgs)`](#fn-specforproviderwithapplyargsmixin)
    * [`fn withDestroyArgs(destroyArgs)`](#fn-specforproviderwithdestroyargs)
    * [`fn withDestroyArgsMixin(destroyArgs)`](#fn-specforproviderwithdestroyargsmixin)
    * [`fn withEnableTofuCLILogging(enableTofuCLILogging)`](#fn-specforproviderwithenabletofuclilogging)
    * [`fn withEntrypoint(entrypoint)`](#fn-specforproviderwithentrypoint)
    * [`fn withEnv(env)`](#fn-specforproviderwithenv)
    * [`fn withEnvMixin(env)`](#fn-specforproviderwithenvmixin)
    * [`fn withInitArgs(initArgs)`](#fn-specforproviderwithinitargs)
    * [`fn withInitArgsMixin(initArgs)`](#fn-specforproviderwithinitargsmixin)
    * [`fn withInlineFormat(inlineFormat)`](#fn-specforproviderwithinlineformat)
    * [`fn withModule(module)`](#fn-specforproviderwithmodule)
    * [`fn withPlanArgs(planArgs)`](#fn-specforproviderwithplanargs)
    * [`fn withPlanArgsMixin(planArgs)`](#fn-specforproviderwithplanargsmixin)
    * [`fn withSource(source)`](#fn-specforproviderwithsource)
    * [`fn withVarFiles(varFiles)`](#fn-specforproviderwithvarfiles)
    * [`fn withVarFilesMixin(varFiles)`](#fn-specforproviderwithvarfilesmixin)
    * [`fn withVarmap(varmap)`](#fn-specforproviderwithvarmap)
    * [`fn withVarmapMixin(varmap)`](#fn-specforproviderwithvarmapmixin)
    * [`fn withVars(vars)`](#fn-specforproviderwithvars)
    * [`fn withVarsMixin(vars)`](#fn-specforproviderwithvarsmixin)
    * [`obj spec.forProvider.env`](#obj-specforproviderenv)
      * [`fn withName(name)`](#fn-specforproviderenvwithname)
      * [`fn withValue(value)`](#fn-specforproviderenvwithvalue)
      * [`obj spec.forProvider.env.configMapKeyRef`](#obj-specforproviderenvconfigmapkeyref)
        * [`fn withKey(key)`](#fn-specforproviderenvconfigmapkeyrefwithkey)
        * [`fn withName(name)`](#fn-specforproviderenvconfigmapkeyrefwithname)
        * [`fn withNamespace(namespace)`](#fn-specforproviderenvconfigmapkeyrefwithnamespace)
      * [`obj spec.forProvider.env.secretKeyRef`](#obj-specforproviderenvsecretkeyref)
        * [`fn withKey(key)`](#fn-specforproviderenvsecretkeyrefwithkey)
        * [`fn withName(name)`](#fn-specforproviderenvsecretkeyrefwithname)
        * [`fn withNamespace(namespace)`](#fn-specforproviderenvsecretkeyrefwithnamespace)
    * [`obj spec.forProvider.varFiles`](#obj-specforprovidervarfiles)
      * [`fn withFormat(format)`](#fn-specforprovidervarfileswithformat)
      * [`fn withSource(source)`](#fn-specforprovidervarfileswithsource)
      * [`obj spec.forProvider.varFiles.configMapKeyRef`](#obj-specforprovidervarfilesconfigmapkeyref)
        * [`fn withKey(key)`](#fn-specforprovidervarfilesconfigmapkeyrefwithkey)
        * [`fn withName(name)`](#fn-specforprovidervarfilesconfigmapkeyrefwithname)
        * [`fn withNamespace(namespace)`](#fn-specforprovidervarfilesconfigmapkeyrefwithnamespace)
      * [`obj spec.forProvider.varFiles.secretKeyRef`](#obj-specforprovidervarfilessecretkeyref)
        * [`fn withKey(key)`](#fn-specforprovidervarfilessecretkeyrefwithkey)
        * [`fn withName(name)`](#fn-specforprovidervarfilessecretkeyrefwithname)
        * [`fn withNamespace(namespace)`](#fn-specforprovidervarfilessecretkeyrefwithnamespace)
    * [`obj spec.forProvider.vars`](#obj-specforprovidervars)
      * [`fn withKey(key)`](#fn-specforprovidervarswithkey)
      * [`fn withValue(value)`](#fn-specforprovidervarswithvalue)
  * [`obj spec.providerConfigRef`](#obj-specproviderconfigref)
    * [`fn withName(name)`](#fn-specproviderconfigrefwithname)
    * [`obj spec.providerConfigRef.policy`](#obj-specproviderconfigrefpolicy)
      * [`fn withResolution(resolution)`](#fn-specproviderconfigrefpolicywithresolution)
      * [`fn withResolve(resolve)`](#fn-specproviderconfigrefpolicywithresolve)
  * [`obj spec.publishConnectionDetailsTo`](#obj-specpublishconnectiondetailsto)
    * [`fn withName(name)`](#fn-specpublishconnectiondetailstowithname)
    * [`obj spec.publishConnectionDetailsTo.configRef`](#obj-specpublishconnectiondetailstoconfigref)
      * [`fn withName(name)`](#fn-specpublishconnectiondetailstoconfigrefwithname)
      * [`obj spec.publishConnectionDetailsTo.configRef.policy`](#obj-specpublishconnectiondetailstoconfigrefpolicy)
        * [`fn withResolution(resolution)`](#fn-specpublishconnectiondetailstoconfigrefpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specpublishconnectiondetailstoconfigrefpolicywithresolve)
    * [`obj spec.publishConnectionDetailsTo.metadata`](#obj-specpublishconnectiondetailstometadata)
      * [`fn withAnnotations(annotations)`](#fn-specpublishconnectiondetailstometadatawithannotations)
      * [`fn withAnnotationsMixin(annotations)`](#fn-specpublishconnectiondetailstometadatawithannotationsmixin)
      * [`fn withLabels(labels)`](#fn-specpublishconnectiondetailstometadatawithlabels)
      * [`fn withLabelsMixin(labels)`](#fn-specpublishconnectiondetailstometadatawithlabelsmixin)
      * [`fn withType(type)`](#fn-specpublishconnectiondetailstometadatawithtype)
  * [`obj spec.writeConnectionSecretToRef`](#obj-specwriteconnectionsecrettoref)
    * [`fn withName(name)`](#fn-specwriteconnectionsecrettorefwithname)
    * [`fn withNamespace(namespace)`](#fn-specwriteconnectionsecrettorefwithnamespace)

## Fields

### fn new

```ts
new(name)
```

new returns an instance of Workspace

## obj metadata

"ObjectMeta is metadata that all persisted resources must have, which includes all objects users must create."

### fn metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

### fn metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

**Note:** This function appends passed data to existing values

### fn metadata.withClusterName

```ts
withClusterName(clusterName)
```

"The name of the cluster which the object belongs to. This is used to distinguish resources with same name and namespace in different clusters. This field is not set anywhere right now and apiserver is going to ignore it if set in create or update request."

### fn metadata.withCreationTimestamp

```ts
withCreationTimestamp(creationTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withDeletionGracePeriodSeconds

```ts
withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)
```

"Number of seconds allowed for this object to gracefully terminate before it will be removed from the system. Only set when deletionTimestamp is also set. May only be shortened. Read-only."

### fn metadata.withDeletionTimestamp

```ts
withDeletionTimestamp(deletionTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withFinalizers

```ts
withFinalizers(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

### fn metadata.withFinalizersMixin

```ts
withFinalizersMixin(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

**Note:** This function appends passed data to existing values

### fn metadata.withGenerateName

```ts
withGenerateName(generateName)
```

"GenerateName is an optional prefix, used by the server, to generate a unique name ONLY IF the Name field has not been provided. If this field is used, the name returned to the client will be different than the name passed. This value will also be combined with a unique suffix. The provided value has the same validation rules as the Name field, and may be truncated by the length of the suffix required to make the value unique on the server.\n\nIf this field is specified and the generated name exists, the server will NOT return a 409 - instead, it will either return 201 Created or 500 with Reason ServerTimeout indicating a unique name could not be found in the time allotted, and the client should retry (optionally after the time indicated in the Retry-After header).\n\nApplied only if Name is not specified. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#idempotency"

### fn metadata.withGeneration

```ts
withGeneration(generation)
```

"A sequence number representing a specific generation of the desired state. Populated by the system. Read-only."

### fn metadata.withLabels

```ts
withLabels(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

### fn metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

**Note:** This function appends passed data to existing values

### fn metadata.withName

```ts
withName(name)
```

"Name must be unique within a namespace. Is required when creating resources, although some resources may allow a client to request the generation of an appropriate name automatically. Name is primarily intended for creation idempotence and configuration definition. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/identifiers#names"

### fn metadata.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the space within which each name must be unique. An empty namespace is equivalent to the \"default\" namespace, but \"default\" is the canonical representation. Not all objects are required to be scoped to a namespace - the value of this field for those objects will be empty.\n\nMust be a DNS_LABEL. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/namespaces"

### fn metadata.withOwnerReferences

```ts
withOwnerReferences(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

### fn metadata.withOwnerReferencesMixin

```ts
withOwnerReferencesMixin(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

**Note:** This function appends passed data to existing values

### fn metadata.withResourceVersion

```ts
withResourceVersion(resourceVersion)
```

"An opaque value that represents the internal version of this object that can be used by clients to determine when objects have changed. May be used for optimistic concurrency, change detection, and the watch operation on a resource or set of resources. Clients must treat these values as opaque and passed unmodified back to the server. They may only be valid for a particular resource or set of resources.\n\nPopulated by the system. Read-only. Value must be treated as opaque by clients and . More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency"

### fn metadata.withSelfLink

```ts
withSelfLink(selfLink)
```

"SelfLink is a URL representing this object. Populated by the system. Read-only.\n\nDEPRECATED Kubernetes will stop propagating this field in 1.20 release and the field is planned to be removed in 1.21 release."

### fn metadata.withUid

```ts
withUid(uid)
```

"UID is the unique in time and space value for this object. It is typically generated by the server on successful creation of a resource and is not allowed to change on PUT operations.\n\nPopulated by the system. Read-only. More info: http://kubernetes.io/docs/user-guide/identifiers#uids"

## obj spec

"A WorkspaceSpec defines the desired state of a Workspace."

### fn spec.withDeletionPolicy

```ts
withDeletionPolicy(deletionPolicy)
```

"DeletionPolicy specifies what will happen to the underlying external\nwhen this managed resource is deleted - either \"Delete\" or \"Orphan\" the\nexternal resource.\nThis field is planned to be deprecated in favor of the ManagementPolicies\nfield in a future release. Currently, both could be set independently and\nnon-default values would be honored if the feature flag is enabled.\nSee the design doc for more information: https://github.com/crossplane/crossplane/blob/499895a25d1a1a0ba1604944ef98ac7a1a71f197/design/design-doc-observe-only-resources.md?plain=1#L223"

### fn spec.withManagementPolicies

```ts
withManagementPolicies(managementPolicies)
```

"THIS IS A BETA FIELD. It is on by default but can be opted out\nthrough a Crossplane feature flag.\nManagementPolicies specify the array of actions Crossplane is allowed to\ntake on the managed and external resources.\nThis field is planned to replace the DeletionPolicy field in a future\nrelease. Currently, both could be set independently and non-default\nvalues would be honored if the feature flag is enabled. If both are\ncustom, the DeletionPolicy field will be ignored.\nSee the design doc for more information: https://github.com/crossplane/crossplane/blob/499895a25d1a1a0ba1604944ef98ac7a1a71f197/design/design-doc-observe-only-resources.md?plain=1#L223\nand this one: https://github.com/crossplane/crossplane/blob/444267e84783136daa93568b364a5f01228cacbe/design/one-pager-ignore-changes.md"

### fn spec.withManagementPoliciesMixin

```ts
withManagementPoliciesMixin(managementPolicies)
```

"THIS IS A BETA FIELD. It is on by default but can be opted out\nthrough a Crossplane feature flag.\nManagementPolicies specify the array of actions Crossplane is allowed to\ntake on the managed and external resources.\nThis field is planned to replace the DeletionPolicy field in a future\nrelease. Currently, both could be set independently and non-default\nvalues would be honored if the feature flag is enabled. If both are\ncustom, the DeletionPolicy field will be ignored.\nSee the design doc for more information: https://github.com/crossplane/crossplane/blob/499895a25d1a1a0ba1604944ef98ac7a1a71f197/design/design-doc-observe-only-resources.md?plain=1#L223\nand this one: https://github.com/crossplane/crossplane/blob/444267e84783136daa93568b364a5f01228cacbe/design/one-pager-ignore-changes.md"

**Note:** This function appends passed data to existing values

## obj spec.forProvider

"WorkspaceParameters are the configurable fields of a Workspace."

### fn spec.forProvider.withApplyArgs

```ts
withApplyArgs(applyArgs)
```

"Arguments to be included in the tofu apply CLI command"

### fn spec.forProvider.withApplyArgsMixin

```ts
withApplyArgsMixin(applyArgs)
```

"Arguments to be included in the tofu apply CLI command"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withDestroyArgs

```ts
withDestroyArgs(destroyArgs)
```

"Arguments to be included in the tofu destroy CLI command"

### fn spec.forProvider.withDestroyArgsMixin

```ts
withDestroyArgsMixin(destroyArgs)
```

"Arguments to be included in the tofu destroy CLI command"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withEnableTofuCLILogging

```ts
withEnableTofuCLILogging(enableTofuCLILogging)
```

"Boolean value to indicate CLI logging of tofu execution is enabled or not"

### fn spec.forProvider.withEntrypoint

```ts
withEntrypoint(entrypoint)
```

"Entrypoint for `tofu init` within the module"

### fn spec.forProvider.withEnv

```ts
withEnv(env)
```

"Environment variables."

### fn spec.forProvider.withEnvMixin

```ts
withEnvMixin(env)
```

"Environment variables."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withInitArgs

```ts
withInitArgs(initArgs)
```

"Arguments to be included in the tofu init CLI command"

### fn spec.forProvider.withInitArgsMixin

```ts
withInitArgsMixin(initArgs)
```

"Arguments to be included in the tofu init CLI command"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withInlineFormat

```ts
withInlineFormat(inlineFormat)
```

"Specifies the format of the inline Terraform content\nif Source is 'Inline'"

### fn spec.forProvider.withModule

```ts
withModule(module)
```

"The root module of this workspace; i.e. the module containing its main.tf\nfile. When the workspace's source is 'Remote' (the default) this can be\nany address supported by tofu init -from-module, for example a git\nrepository or an S3 bucket. When the workspace's source is 'Inline' the\ncontent of a simple main.tf or main.tf.json file may be written inline."

### fn spec.forProvider.withPlanArgs

```ts
withPlanArgs(planArgs)
```

"Arguments to be included in the tofu plan CLI command"

### fn spec.forProvider.withPlanArgsMixin

```ts
withPlanArgsMixin(planArgs)
```

"Arguments to be included in the tofu plan CLI command"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withSource

```ts
withSource(source)
```

"Source of the root module of this workspace."

### fn spec.forProvider.withVarFiles

```ts
withVarFiles(varFiles)
```

"Files of configuration variables. Explicitly declared vars take\nprecedence."

### fn spec.forProvider.withVarFilesMixin

```ts
withVarFilesMixin(varFiles)
```

"Files of configuration variables. Explicitly declared vars take\nprecedence."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withVarmap

```ts
withVarmap(varmap)
```

"Terraform Variable Map. Should be a valid JSON representation of the input vars"

### fn spec.forProvider.withVarmapMixin

```ts
withVarmapMixin(varmap)
```

"Terraform Variable Map. Should be a valid JSON representation of the input vars"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withVars

```ts
withVars(vars)
```

"Configuration variables."

### fn spec.forProvider.withVarsMixin

```ts
withVarsMixin(vars)
```

"Configuration variables."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.env

"Environment variables."

### fn spec.forProvider.env.withName

```ts
withName(name)
```



### fn spec.forProvider.env.withValue

```ts
withValue(value)
```



## obj spec.forProvider.env.configMapKeyRef

"A ConfigMap key containing the desired env var value."

### fn spec.forProvider.env.configMapKeyRef.withKey

```ts
withKey(key)
```

"Key within the referenced resource."

### fn spec.forProvider.env.configMapKeyRef.withName

```ts
withName(name)
```

"Name of the referenced resource."

### fn spec.forProvider.env.configMapKeyRef.withNamespace

```ts
withNamespace(namespace)
```

"Namespace of the referenced resource."

## obj spec.forProvider.env.secretKeyRef

"A Secret key containing the desired env var value."

### fn spec.forProvider.env.secretKeyRef.withKey

```ts
withKey(key)
```

"Key within the referenced resource."

### fn spec.forProvider.env.secretKeyRef.withName

```ts
withName(name)
```

"Name of the referenced resource."

### fn spec.forProvider.env.secretKeyRef.withNamespace

```ts
withNamespace(namespace)
```

"Namespace of the referenced resource."

## obj spec.forProvider.varFiles

"Files of configuration variables. Explicitly declared vars take\nprecedence."

### fn spec.forProvider.varFiles.withFormat

```ts
withFormat(format)
```

"Format of this vars file."

### fn spec.forProvider.varFiles.withSource

```ts
withSource(source)
```

"Source of this vars file."

## obj spec.forProvider.varFiles.configMapKeyRef

"A ConfigMap key containing the vars file."

### fn spec.forProvider.varFiles.configMapKeyRef.withKey

```ts
withKey(key)
```

"Key within the referenced resource."

### fn spec.forProvider.varFiles.configMapKeyRef.withName

```ts
withName(name)
```

"Name of the referenced resource."

### fn spec.forProvider.varFiles.configMapKeyRef.withNamespace

```ts
withNamespace(namespace)
```

"Namespace of the referenced resource."

## obj spec.forProvider.varFiles.secretKeyRef

"A Secret key containing the vars file."

### fn spec.forProvider.varFiles.secretKeyRef.withKey

```ts
withKey(key)
```

"Key within the referenced resource."

### fn spec.forProvider.varFiles.secretKeyRef.withName

```ts
withName(name)
```

"Name of the referenced resource."

### fn spec.forProvider.varFiles.secretKeyRef.withNamespace

```ts
withNamespace(namespace)
```

"Namespace of the referenced resource."

## obj spec.forProvider.vars

"Configuration variables."

### fn spec.forProvider.vars.withKey

```ts
withKey(key)
```



### fn spec.forProvider.vars.withValue

```ts
withValue(value)
```



## obj spec.providerConfigRef

"ProviderConfigReference specifies how the provider that will be used to\ncreate, observe, update, and delete this managed resource should be\nconfigured."

### fn spec.providerConfigRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.providerConfigRef.policy

"Policies for referencing."

### fn spec.providerConfigRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.providerConfigRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.publishConnectionDetailsTo

"PublishConnectionDetailsTo specifies the connection secret config which\ncontains a name, metadata and a reference to secret store config to\nwhich any connection details for this managed resource should be written.\nConnection details frequently include the endpoint, username,\nand password required to connect to the managed resource."

### fn spec.publishConnectionDetailsTo.withName

```ts
withName(name)
```

"Name is the name of the connection secret."

## obj spec.publishConnectionDetailsTo.configRef

"SecretStoreConfigRef specifies which secret store config should be used\nfor this ConnectionSecret."

### fn spec.publishConnectionDetailsTo.configRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.publishConnectionDetailsTo.configRef.policy

"Policies for referencing."

### fn spec.publishConnectionDetailsTo.configRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.publishConnectionDetailsTo.configRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.publishConnectionDetailsTo.metadata

"Metadata is the metadata for connection secret."

### fn spec.publishConnectionDetailsTo.metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations are the annotations to be added to connection secret.\n- For Kubernetes secrets, this will be used as \"metadata.annotations\".\n- It is up to Secret Store implementation for others store types."

### fn spec.publishConnectionDetailsTo.metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations are the annotations to be added to connection secret.\n- For Kubernetes secrets, this will be used as \"metadata.annotations\".\n- It is up to Secret Store implementation for others store types."

**Note:** This function appends passed data to existing values

### fn spec.publishConnectionDetailsTo.metadata.withLabels

```ts
withLabels(labels)
```

"Labels are the labels/tags to be added to connection secret.\n- For Kubernetes secrets, this will be used as \"metadata.labels\".\n- It is up to Secret Store implementation for others store types."

### fn spec.publishConnectionDetailsTo.metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Labels are the labels/tags to be added to connection secret.\n- For Kubernetes secrets, this will be used as \"metadata.labels\".\n- It is up to Secret Store implementation for others store types."

**Note:** This function appends passed data to existing values

### fn spec.publishConnectionDetailsTo.metadata.withType

```ts
withType(type)
```

"Type is the SecretType for the connection secret.\n- Only valid for Kubernetes Secret Stores."

## obj spec.writeConnectionSecretToRef

"WriteConnectionSecretToReference specifies the namespace and name of a\nSecret to which any connection details for this managed resource should\nbe written. Connection details frequently include the endpoint, username,\nand password required to connect to the managed resource.\nThis field is planned to be replaced in a future release in favor of\nPublishConnectionDetailsTo. Currently, both could be set independently\nand connection details would be published to both without affecting\neach other."

### fn spec.writeConnectionSecretToRef.withName

```ts
withName(name)
```

"Name of the secret."

### fn spec.writeConnectionSecretToRef.withNamespace

```ts
withNamespace(namespace)
```

"Namespace of the secret."