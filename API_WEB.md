## Modules

<dl>
<dt><a href="#module_Descriptor">Descriptor</a> ⇒ <code>Array.&lt;String&gt;</code></dt>
<dd><p>Describe an archive dataset - to history commands</p>
</dd>
<dt><a href="#module_command">command</a></dt>
<dd><p>Command related tools</p>
</dd>
</dl>

## Classes

<dl>
<dt><a href="#Archive">Archive</a></dt>
<dd></dd>
<dt><a href="#Comparator">Comparator</a></dt>
<dd></dd>
<dt><a href="#ArchiveManager">ArchiveManager</a></dt>
<dd><p>Archive manager for managing archives and connections to sources</p>
</dd>
<dt><a href="#DropboxDatasource">DropboxDatasource</a> ⇐ <code><a href="#TextDatasource">TextDatasource</a></code></dt>
<dd><p>Datasource for Dropbox archives</p>
</dd>
<dt><a href="#Entry">Entry</a></dt>
<dd></dd>
<dt><a href="#EntryFinder">EntryFinder</a></dt>
<dd><p>Entry searching class</p>
</dd>
<dt><a href="#FileDatasource">FileDatasource</a> ⇐ <code><a href="#TextDatasource">TextDatasource</a></code></dt>
<dd></dd>
<dt><a href="#FileDatasource">FileDatasource</a></dt>
<dd></dd>
<dt><a href="#Flattener">Flattener</a></dt>
<dd></dd>
<dt><a href="#Group">Group</a></dt>
<dd></dd>
<dt><a href="#Group">Group</a></dt>
<dd></dd>
<dt><a href="#Model">Model</a></dt>
<dd></dd>
<dt><a href="#MyButtercupDatasource">MyButtercupDatasource</a> ⇐ <code><a href="#TextDatasource">TextDatasource</a></code></dt>
<dd><p>Datasource for the MyButtercup provider</p>
</dd>
<dt><a href="#NextcloudDatasource">NextcloudDatasource</a> ⇐ <code><a href="#OwnCloudDatasource">OwnCloudDatasource</a></code></dt>
<dd><p>Datasource for Nextcloud archives</p>
</dd>
<dt><a href="#OwnCloudDatasource">OwnCloudDatasource</a> ⇐ <code><a href="#WebDAVDatasource">WebDAVDatasource</a></code></dt>
<dd><p>Datasource for OwnCloud archives</p>
</dd>
<dt><a href="#TextDatasource">TextDatasource</a></dt>
<dd><p>Datasource for text input and output</p>
</dd>
<dt><a href="#WebDAVDatasource">WebDAVDatasource</a> ⇐ <code><a href="#TextDatasource">TextDatasource</a></code></dt>
<dd></dd>
<dt><a href="#WebDAVDatasource">WebDAVDatasource</a></dt>
<dd></dd>
<dt><a href="#Westley">Westley</a></dt>
<dd></dd>
<dt><a href="#Workspace">Workspace</a></dt>
<dd></dd>
<dt><a href="#LocalStorageInterface">LocalStorageInterface</a> ⇐ <code>StorageInterface</code></dt>
<dd><p>Interface for localStorage</p>
</dd>
</dl>

## Mixins

<dl>
<dt><a href="#EntryCollection">EntryCollection</a> : <code>Object</code></dt>
<dd></dd>
<dt><a href="#GroupCollection">GroupCollection</a> : <code>Object</code></dt>
<dd></dd>
</dl>

## Functions

<dl>
<dt><a href="#flattenEntries">flattenEntries(archives)</a> ⇒ <code><a href="#EntrySearchInfo">Array.&lt;EntrySearchInfo&gt;</a></code></dt>
<dd><p>Flatten entries into a searchable structure</p>
</dd>
<dt><a href="#convertEncryptedContentToHistory">convertEncryptedContentToHistory(encText, credentials)</a> ⇒ <code>Promise.&lt;Array&gt;</code></dt>
<dd><p>Convert encrypted text to an array of commands (history)</p>
</dd>
<dt><a href="#convertHistoryToEncryptedContent">convertHistoryToEncryptedContent(historyArr, credentials)</a> ⇒ <code>String</code></dt>
<dd><p>Convert an array of commands (history) to an encrypted string</p>
</dd>
<dt><a href="#createCredentials">createCredentials([type], [data])</a> ⇒ <code><a href="#Credentials">Credentials</a></code></dt>
<dd><p>Create a credentials adapter
Both <code>type</code> and <code>data</code> parameters are optional.</p>
</dd>
<dt><a href="#addMetaFieldsNonDestructive">addMetaFieldsNonDestructive(entry, fields)</a> ⇒ <code><a href="#EntryFacadeField">Array.&lt;EntryFacadeField&gt;</a></code></dt>
<dd><p>Add meta fields to a fields array that are not mentioned in a preset
Facades are creaded by presets which don&#39;t mention all meta values (custom user
added items). This method adds the unmentioned items to the facade fields so that
they can be edited as well.</p>
</dd>
<dt><a href="#applyFieldDescriptor">applyFieldDescriptor(entry, descriptor)</a></dt>
<dd><p>Apply a facade field descriptor to an entry
Takes data from the descriptor and writes it to the entry.</p>
</dd>
<dt><a href="#consumeEntryFacade">consumeEntryFacade(entry, facade)</a></dt>
<dd><p>Process a modified entry facade</p>
</dd>
<dt><a href="#createEntryFacade">createEntryFacade(entry)</a> ⇒ <code><a href="#EntryFacade">EntryFacade</a></code></dt>
<dd><p>Create a data/input facade for an Entry instance</p>
</dd>
<dt><a href="#getEntryFacadeType">getEntryFacadeType(entry)</a> ⇒ <code>String</code></dt>
<dd><p>Get the facade type for an entry</p>
</dd>
<dt><a href="#setEntryValue">setEntryValue(entry, property, name, value)</a></dt>
<dd><p>Set a value on an entry</p>
</dd>
<dt><a href="#dedupe">dedupe(arr)</a> ⇒ <code>Array</code></dt>
<dd><p>De-dupe an array</p>
</dd>
<dt><a href="#createFieldDescriptor">createFieldDescriptor(entry, title, entryPropertyType, entryPropertyName, options)</a> ⇒ <code><a href="#EntryFacadeField">EntryFacadeField</a></code></dt>
<dd><p>Create a descriptor for a field to be used within a facade</p>
</dd>
<dt><a href="#getEntryValue">getEntryValue(entry, property, name)</a> ⇒ <code>String</code></dt>
<dd><p>Get a value on an entry for a specific property type</p>
</dd>
<dt><a href="#getValidProperties">getValidProperties()</a> ⇒ <code>Array.&lt;String&gt;</code></dt>
<dd><p>Get an array of valid property names</p>
</dd>
<dt><a href="#isValidProperty">isValidProperty(name)</a> ⇒ <code>Boolean</code></dt>
<dd><p>Check if a property name is valid</p>
</dd>
<dt><a href="#generateUUID">generateUUID()</a> ⇒ <code>String</code></dt>
<dd><p>Generate a UUID (v4)</p>
</dd>
<dt><a href="#findEntriesByCheck">findEntriesByCheck(groups, compareFn)</a> ⇒ <code><a href="#Entry">Array.&lt;Entry&gt;</a></code></dt>
<dd><p>Find entry instances by filtering with a compare function</p>
</dd>
<dt><a href="#findGroupsByCheck">findGroupsByCheck(groups, compareFn)</a> ⇒ <code><a href="#Group">Array.&lt;Group&gt;</a></code></dt>
<dd><p>Find group instances within groups that satisfy some check</p>
</dd>
<dt><a href="#getAllEntries">getAllEntries(groups)</a> ⇒ <code><a href="#Entry">Array.&lt;Entry&gt;</a></code></dt>
<dd><p>Get all entries within a collection of groups</p>
</dd>
<dt><a href="#deriveKeyFromPassword">deriveKeyFromPassword(password, salt, rounds, bits)</a> ⇒ <code>Promise.&lt;ArrayBuffer&gt;</code></dt>
<dd><p>Derive a key from a password</p>
</dd>
<dt><a href="#patchCorePBKDF">patchCorePBKDF(handler)</a></dt>
<dd><p>Perform patching of the PBKDF2 function in iocane</p>
</dd>
</dl>

## Typedefs

<dl>
<dt><a href="#ArchiveManagerSourceStatus">ArchiveManagerSourceStatus</a> : <code>String</code></dt>
<dd><p>Status of a source: locked/unlocked/pending</p>
</dd>
<dt><a href="#UnlockedArchiveManagerSource">UnlockedArchiveManagerSource</a> : <code>Object</code></dt>
<dd></dd>
<dt><a href="#LockedArchiveManagerSource">LockedArchiveManagerSource</a> : <code>Object</code></dt>
<dd></dd>
<dt><a href="#EntrySearchInfo">EntrySearchInfo</a> : <code>Object</code></dt>
<dd></dd>
<dt><a href="#WorkspaceItem">WorkspaceItem</a> : <code>Object</code></dt>
<dd><p>Shared workspace item</p>
</dd>
<dt><a href="#Credentials">Credentials</a> : <code>Object</code></dt>
<dd><p>Credentials wrapper</p>
</dd>
<dt><a href="#EntryFacade">EntryFacade</a> : <code>Object</code></dt>
<dd><p>Entry facade for data input</p>
</dd>
<dt><a href="#EntryFacadeField">EntryFacadeField</a> : <code>Object</code></dt>
<dd><p>Entry facade data field</p>
</dd>
<dt><a href="#FoundGroupResult">FoundGroupResult</a> : <code>Object</code></dt>
<dd></dd>
</dl>

<a name="module_Descriptor"></a>

## Descriptor ⇒ <code>Array.&lt;String&gt;</code>
Describe an archive dataset - to history commands

**Returns**: <code>Array.&lt;String&gt;</code> - An array of commands  

| Param | Type | Description |
| --- | --- | --- |
| dataset | <code>Object</code> | The archive dataset |
| parentGroupID | <code>String</code> | The ID of the parent group |

<a name="module_command"></a>

## command
Command related tools

<a name="module_command.extractCommandComponents"></a>

### command.extractCommandComponents(command) ⇒ <code>Array.&lt;String&gt;</code>
Extract command components from a string

**Kind**: static method of <code>[command](#module_command)</code>  
**Returns**: <code>Array.&lt;String&gt;</code> - The separated parts  

| Param | Type | Description |
| --- | --- | --- |
| command | <code>String</code> | The command to extract from |

<a name="Archive"></a>

## Archive
**Kind**: global class  
**Mixes**: <code>[GroupCollection](#GroupCollection)</code>, <code>[EntryCollection](#EntryCollection)</code>  

* [Archive](#Archive)
    * [new Archive()](#new_Archive_new)
    * _instance_
        * [.readOnly](#Archive+readOnly)
        * [.sharedGroups](#Archive+sharedGroups)
        * [.type](#Archive+type) : <code>String</code>
        * [.findGroupByID](#Archive+findGroupByID) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
        * [.findGroupsByTitle](#Archive+findGroupsByTitle) ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
        * [.findEntriesByMeta](#Archive+findEntriesByMeta) ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
        * [.findEntriesByProperty](#Archive+findEntriesByProperty) ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
        * [.createGroup([title])](#Archive+createGroup) ⇒ <code>[Group](#Group)</code>
        * [.deleteAttribute(attributeName)](#Archive+deleteAttribute) ⇒ <code>[Archive](#Archive)</code>
        * [.discardSharedGroups()](#Archive+discardSharedGroups) ⇒ <code>[Archive](#Archive)</code>
        * [.emptyTrash()](#Archive+emptyTrash)
        * [.getAttribute(attributeName)](#Archive+getAttribute) ⇒ <code>undefined</code> &#124; <code>String</code>
        * [.getAttributes()](#Archive+getAttributes) ⇒ <code>Object</code>
        * [.getEntryByID(entryID)](#Archive+getEntryByID) ⇒ <code>[Entry](#Entry)</code> &#124; <code>null</code>
        * [.getFormat()](#Archive+getFormat) ⇒ <code>string</code>
        * ~~[.getGroupByID(groupID)](#Archive+getGroupByID) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>~~
        * [.getGroups()](#Archive+getGroups) ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
        * [.getHistory()](#Archive+getHistory) ⇒ <code>Array.&lt;String&gt;</code>
        * [.getID()](#Archive+getID) ⇒ <code>String</code>
        * [.getTrashGroup()](#Archive+getTrashGroup) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
        * [.optimise()](#Archive+optimise) ⇒ <code>[Archive](#Archive)</code>
        * [.setAttribute(attributeName, value)](#Archive+setAttribute) ⇒ <code>[Archive](#Archive)</code>
        * [.toObject(groupOutputFlags)](#Archive+toObject) ⇒ <code>Object</code>
        * [._generateID()](#Archive+_generateID)
        * [._getWestley()](#Archive+_getWestley) ⇒ <code>[Westley](#Westley)</code>
        * [.inst.findEntryByID(id)](#Archive+findEntryByID) ⇒ <code>null</code> &#124; <code>[Entry](#Entry)</code>
    * _static_
        * [.createFromHistory(history)](#Archive.createFromHistory) ⇒ <code>[Archive](#Archive)</code>
        * [.createWithDefaults()](#Archive.createWithDefaults) ⇒ <code>[Archive](#Archive)</code>

<a name="new_Archive_new"></a>

### new Archive()
Buttercup Archive

<a name="Archive+readOnly"></a>

### archive.readOnly
Whether the archive is read only or not

**Kind**: instance property of <code>[Archive](#Archive)</code>  
**Read only**: true  
**Properties**

| Name | Type |
| --- | --- |
| readOnly | <code>Boolean</code> | 

<a name="Archive+sharedGroups"></a>

### archive.sharedGroups
An array of shared groups

**Kind**: instance property of <code>[Archive](#Archive)</code>  
**Properties**

| Name | Type |
| --- | --- |
| sharedGroups | <code>[Array.&lt;Group&gt;](#Group)</code> | 

<a name="Archive+type"></a>

### archive.type : <code>String</code>
Get the instance type

**Kind**: instance property of <code>[Archive](#Archive)</code>  
<a name="Archive+findGroupByID"></a>

### archive.findGroupByID ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
Find a group by its ID

**Kind**: instance property of <code>[Archive](#Archive)</code>  
**Mixes**: <code>[findGroupByID](#GroupCollection.findGroupByID)</code>  
**Returns**: <code>[Group](#Group)</code> &#124; <code>null</code> - The group or null if not found  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The group ID to search for |

<a name="Archive+findGroupsByTitle"></a>

### archive.findGroupsByTitle ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
Find groups by their title

**Kind**: instance property of <code>[Archive](#Archive)</code>  
**Mixes**: <code>[findGroupsByTitle](#GroupCollection.findGroupsByTitle)</code>  
**Returns**: <code>[Array.&lt;Group&gt;](#Group)</code> - An array of groups  

| Param | Type | Description |
| --- | --- | --- |
| title | <code>String</code> &#124; <code>RegExp</code> | The group title |

<a name="Archive+findEntriesByMeta"></a>

### archive.findEntriesByMeta ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
Find entries that match a certain meta property

**Kind**: instance property of <code>[Archive](#Archive)</code>  
**Mixes**: <code>[findEntriesByMeta](#EntryCollection.findEntriesByMeta)</code>  
**Returns**: <code>[Array.&lt;Entry&gt;](#Entry)</code> - An array of found entries  

| Param | Type | Description |
| --- | --- | --- |
| metaName | <code>String</code> | The meta property to search for |
| value | <code>RegExp</code> &#124; <code>string</code> | The value to search for |

<a name="Archive+findEntriesByProperty"></a>

### archive.findEntriesByProperty ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
Find all entries that match a certain property

**Kind**: instance property of <code>[Archive](#Archive)</code>  
**Mixes**: <code>[findEntriesByProperty](#EntryCollection.findEntriesByProperty)</code>  
**Returns**: <code>[Array.&lt;Entry&gt;](#Entry)</code> - An array of found extries  

| Param | Type | Description |
| --- | --- | --- |
| property | <code>string</code> | The property to search with |
| value | <code>RegExp</code> &#124; <code>string</code> | The value to search for |

<a name="Archive+createGroup"></a>

### archive.createGroup([title]) ⇒ <code>[Group](#Group)</code>
Create a new group

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>[Group](#Group)</code> - The newly created group  

| Param | Type | Description |
| --- | --- | --- |
| [title] | <code>string</code> | The title for the group |

<a name="Archive+deleteAttribute"></a>

### archive.deleteAttribute(attributeName) ⇒ <code>[Archive](#Archive)</code>
Delete an attribute

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>[Archive](#Archive)</code> - Self  

| Param | Type | Description |
| --- | --- | --- |
| attributeName | <code>String</code> | The name of the attribute to delete |

<a name="Archive+discardSharedGroups"></a>

### archive.discardSharedGroups() ⇒ <code>[Archive](#Archive)</code>
Clear the shared groups array

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>[Archive](#Archive)</code> - Self  
<a name="Archive+emptyTrash"></a>

### archive.emptyTrash()
Remove all entries and groups from the trash (permanent)

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Throws**:

- <code>Error</code> Throws if there is no trash group

<a name="Archive+getAttribute"></a>

### archive.getAttribute(attributeName) ⇒ <code>undefined</code> &#124; <code>String</code>
Get the value of an attribute

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>undefined</code> &#124; <code>String</code> - The value of the attribute or undefined if not set  

| Param | Type | Description |
| --- | --- | --- |
| attributeName | <code>String</code> | The attribute to get |

<a name="Archive+getAttributes"></a>

### archive.getAttributes() ⇒ <code>Object</code>
Get all attributes

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>Object</code> - Attributes object  
<a name="Archive+getEntryByID"></a>

### archive.getEntryByID(entryID) ⇒ <code>[Entry](#Entry)</code> &#124; <code>null</code>
Find an entry by its ID

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>[Entry](#Entry)</code> &#124; <code>null</code> - The found entry or null  

| Param | Type | Description |
| --- | --- | --- |
| entryID | <code>String</code> | The entry's ID |

<a name="Archive+getFormat"></a>

### archive.getFormat() ⇒ <code>string</code>
Get the archive format

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>string</code> - The format of the archive  
<a name="Archive+getGroupByID"></a>

### ~~archive.getGroupByID(groupID) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>~~
***Deprecated***

Find a group by its ID

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>[Group](#Group)</code> &#124; <code>null</code> - The group with the provided ID  
**See**: findGroupByID  

| Param | Type | Description |
| --- | --- | --- |
| groupID | <code>String</code> | The group's ID |

<a name="Archive+getGroups"></a>

### archive.getGroups() ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
Get all groups (root) in the archive

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>[Array.&lt;Group&gt;](#Group)</code> - An array of Groups  
<a name="Archive+getHistory"></a>

### archive.getHistory() ⇒ <code>Array.&lt;String&gt;</code>
Get the command array (history)
Returned object can be quite large.

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>Array.&lt;String&gt;</code> - The command array  
<a name="Archive+getID"></a>

### archive.getID() ⇒ <code>String</code>
Get the archive ID

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>String</code> - The ID or an empty string if not set  
<a name="Archive+getTrashGroup"></a>

### archive.getTrashGroup() ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
Get the trash group

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>[Group](#Group)</code> &#124; <code>null</code> - The trash group if found, null otherwise  
<a name="Archive+optimise"></a>

### archive.optimise() ⇒ <code>[Archive](#Archive)</code>
Perform archive optimisations

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>[Archive](#Archive)</code> - Self  
<a name="Archive+setAttribute"></a>

### archive.setAttribute(attributeName, value) ⇒ <code>[Archive](#Archive)</code>
Set an attribute on the archive

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>[Archive](#Archive)</code> - Self  

| Param | Type | Description |
| --- | --- | --- |
| attributeName | <code>String</code> | The attribute to set |
| value | <code>String</code> | The value to set for the attribute |

<a name="Archive+toObject"></a>

### archive.toObject(groupOutputFlags) ⇒ <code>Object</code>
Convert the archive to an object

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>Object</code> - The archive in object form  
**See**: Group.toObject  

| Param | Type | Description |
| --- | --- | --- |
| groupOutputFlags | <code>Number</code> | Bitwise flags for `Group.toObject` |

<a name="Archive+_generateID"></a>

### archive._generateID()
Generate an archive ID

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Access:** protected  
<a name="Archive+_getWestley"></a>

### archive._getWestley() ⇒ <code>[Westley](#Westley)</code>
Get the underlying Westley instance

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Returns**: <code>[Westley](#Westley)</code> - The Westley instance  
**Access:** protected  
<a name="Archive+findEntryByID"></a>

### archive.inst.findEntryByID(id) ⇒ <code>null</code> &#124; <code>[Entry](#Entry)</code>
Find an entry by its ID

**Kind**: instance method of <code>[Archive](#Archive)</code>  
**Mixes**: <code>[inst.findEntryByID](#EntryCollection.inst.findEntryByID)</code>  
**Returns**: <code>null</code> &#124; <code>[Entry](#Entry)</code> - Null if not found, or the Entry instance  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The ID to search for |

<a name="Archive.createFromHistory"></a>

### Archive.createFromHistory(history) ⇒ <code>[Archive](#Archive)</code>
Create a new archive instance from a list of commands (history)

**Kind**: static method of <code>[Archive](#Archive)</code>  
**Returns**: <code>[Archive](#Archive)</code> - The archive instance  

| Param | Type | Description |
| --- | --- | --- |
| history | <code>Array.&lt;String&gt;</code> | The command list |

<a name="Archive.createWithDefaults"></a>

### Archive.createWithDefaults() ⇒ <code>[Archive](#Archive)</code>
Create an Archive with the default template

**Kind**: static method of <code>[Archive](#Archive)</code>  
**Returns**: <code>[Archive](#Archive)</code> - The new archive  
<a name="Comparator"></a>

## Comparator
**Kind**: global class  

* [Comparator](#Comparator)
    * [new Comparator(originalArchive, secondaryArchive)](#new_Comparator_new)
    * [.archivesDiffer()](#Comparator+archivesDiffer) ⇒ <code>Boolean</code>
    * [.calculateDifferences()](#Comparator+calculateDifferences) ⇒ <code>Object</code> &#124; <code>Boolean</code>

<a name="new_Comparator_new"></a>

### new Comparator(originalArchive, secondaryArchive)
Archive comparison class


| Param | Type | Description |
| --- | --- | --- |
| originalArchive | <code>[Archive](#Archive)</code> | The primary archive |
| secondaryArchive | <code>[Archive](#Archive)</code> | The secondary archive |

<a name="Comparator+archivesDiffer"></a>

### comparator.archivesDiffer() ⇒ <code>Boolean</code>
Check if the current archives differ

**Kind**: instance method of <code>[Comparator](#Comparator)</code>  
**Returns**: <code>Boolean</code> - True if the archives are different  
<a name="Comparator+calculateDifferences"></a>

### comparator.calculateDifferences() ⇒ <code>Object</code> &#124; <code>Boolean</code>
Calculate the differences, in commands, between the two archives

**Kind**: instance method of <code>[Comparator](#Comparator)</code>  
**Returns**: <code>Object</code> &#124; <code>Boolean</code> - Returns false if no common base
       is found, or the command differences as two arrays  
<a name="ArchiveManager"></a>

## ArchiveManager
Archive manager for managing archives and connections to sources

**Kind**: global class  

* [ArchiveManager](#ArchiveManager)
    * [new ArchiveManager([storageInterface])](#new_ArchiveManager_new)
    * [.sources](#ArchiveManager+sources) : <code>Array.&lt;(UnlockedArchiveManagerSource\|LockedArchiveManagerSource)&gt;</code>
    * [.storageInterface](#ArchiveManager+storageInterface) : <code>StorageInterface</code>
    * [.unlockedSources](#ArchiveManager+unlockedSources) : <code>Array.&lt;(UnlockedArchiveManagerSource\|LockedArchiveManagerSource)&gt;</code>
    * [.addSource(name, sourceCredentials, archiveCredentials, [initialise])](#ArchiveManager+addSource) ⇒ <code>Promise.&lt;String&gt;</code>
    * [.dehydrateSource(id)](#ArchiveManager+dehydrateSource) ⇒ <code>Promise</code>
    * [.indexOfSource(id)](#ArchiveManager+indexOfSource) ⇒ <code>Number</code>
    * [.lock(id)](#ArchiveManager+lock) ⇒ <code>Promise</code>
    * [.rehydrate()](#ArchiveManager+rehydrate) ⇒ <code>Promise</code>
    * [.remove(id)](#ArchiveManager+remove) ⇒ <code>Promise</code>
    * [.unlock(id, masterPassword)](#ArchiveManager+unlock) ⇒ <code>Promise</code>
    * [._replace(id, source)](#ArchiveManager+_replace)

<a name="new_ArchiveManager_new"></a>

### new ArchiveManager([storageInterface])
Constructor for ArchiveManager


| Param | Type | Description |
| --- | --- | --- |
| [storageInterface] | <code>StorageInterface</code> | An optional StorageInterface instance. Defaults  to a new MemoryStorageInterface instance if not provided |

<a name="ArchiveManager+sources"></a>

### archiveManager.sources : <code>Array.&lt;(UnlockedArchiveManagerSource\|LockedArchiveManagerSource)&gt;</code>
All sources handled by the manager

**Kind**: instance property of <code>[ArchiveManager](#ArchiveManager)</code>  
<a name="ArchiveManager+storageInterface"></a>

### archiveManager.storageInterface : <code>StorageInterface</code>
Reference to the storage interface

**Kind**: instance property of <code>[ArchiveManager](#ArchiveManager)</code>  
<a name="ArchiveManager+unlockedSources"></a>

### archiveManager.unlockedSources : <code>Array.&lt;(UnlockedArchiveManagerSource\|LockedArchiveManagerSource)&gt;</code>
Array of unlocked sources

**Kind**: instance property of <code>[ArchiveManager](#ArchiveManager)</code>  
<a name="ArchiveManager+addSource"></a>

### archiveManager.addSource(name, sourceCredentials, archiveCredentials, [initialise]) ⇒ <code>Promise.&lt;String&gt;</code>
Add a new source

**Kind**: instance method of <code>[ArchiveManager](#ArchiveManager)</code>  
**Returns**: <code>Promise.&lt;String&gt;</code> - A promise that resolves with the source's new ID  

| Param | Type | Default | Description |
| --- | --- | --- | --- |
| name | <code>String</code> |  | The name of the source |
| sourceCredentials | <code>[Credentials](#Credentials)</code> |  | Archive source credentials (remote system) |
| archiveCredentials | <code>[Credentials](#Credentials)</code> |  | Credentials for unlocking the archive |
| [initialise] | <code>Boolean</code> | <code>false</code> | Optionally initialise a blank archive (defaults to false) |

<a name="ArchiveManager+dehydrateSource"></a>

### archiveManager.dehydrateSource(id) ⇒ <code>Promise</code>
Dehydrate a source and write it to storage
Does not lock the source

**Kind**: instance method of <code>[ArchiveManager](#ArchiveManager)</code>  
**Returns**: <code>Promise</code> - A promise that resolves once dehydration has completed  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The ID of the source to lock |

<a name="ArchiveManager+indexOfSource"></a>

### archiveManager.indexOfSource(id) ⇒ <code>Number</code>
Get an index for a source with an ID

**Kind**: instance method of <code>[ArchiveManager](#ArchiveManager)</code>  
**Returns**: <code>Number</code> - The index or -1 if not found  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The ID of the source |

<a name="ArchiveManager+lock"></a>

### archiveManager.lock(id) ⇒ <code>Promise</code>
Lock a source by its ID

**Kind**: instance method of <code>[ArchiveManager](#ArchiveManager)</code>  
**Returns**: <code>Promise</code> - A promise that resolves once the source is locked  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The ID of the source |

<a name="ArchiveManager+rehydrate"></a>

### archiveManager.rehydrate() ⇒ <code>Promise</code>
Rehydrate all sources from storage

**Kind**: instance method of <code>[ArchiveManager](#ArchiveManager)</code>  
**Returns**: <code>Promise</code> - A promise that resolves once all sources have been rehydrated  
<a name="ArchiveManager+remove"></a>

### archiveManager.remove(id) ⇒ <code>Promise</code>
Remove a source

**Kind**: instance method of <code>[ArchiveManager](#ArchiveManager)</code>  
**Returns**: <code>Promise</code> - A promise that resolves once the source has been removed  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The source ID |

<a name="ArchiveManager+unlock"></a>

### archiveManager.unlock(id, masterPassword) ⇒ <code>Promise</code>
Unlock a source

**Kind**: instance method of <code>[ArchiveManager](#ArchiveManager)</code>  
**Returns**: <code>Promise</code> - A promise that resolves once the source is unlocked  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The ID of the source to unlock |
| masterPassword | <code>String</code> | The password to unlock the source |

<a name="ArchiveManager+_replace"></a>

### archiveManager._replace(id, source)
Replace a source by its ID

**Kind**: instance method of <code>[ArchiveManager](#ArchiveManager)</code>  
**Access:** protected  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The ID of the source |
| source | <code>[UnlockedArchiveManagerSource](#UnlockedArchiveManagerSource)</code> &#124; <code>[LockedArchiveManagerSource](#LockedArchiveManagerSource)</code> | The source to replace it with |

<a name="DropboxDatasource"></a>

## DropboxDatasource ⇐ <code>[TextDatasource](#TextDatasource)</code>
Datasource for Dropbox archives

**Kind**: global class  
**Extends:** <code>[TextDatasource](#TextDatasource)</code>  

* [DropboxDatasource](#DropboxDatasource) ⇐ <code>[TextDatasource](#TextDatasource)</code>
    * [new DropboxDatasource(accessToken, resourcePath)](#new_DropboxDatasource_new)
    * [.load(credentials)](#DropboxDatasource+load) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
    * [.save(archive, credentials)](#DropboxDatasource+save) ⇒ <code>Promise</code>
    * [.toObject()](#DropboxDatasource+toObject) ⇒ <code>Object</code>
    * [.setContent(content)](#TextDatasource+setContent) ⇒ <code>[TextDatasource](#TextDatasource)</code>
    * [.toString()](#TextDatasource+toString) ⇒ <code>String</code>

<a name="new_DropboxDatasource_new"></a>

### new DropboxDatasource(accessToken, resourcePath)
Datasource for Dropbox accounts


| Param | Type | Description |
| --- | --- | --- |
| accessToken | <code>String</code> | The dropbox access token |
| resourcePath | <code>String</code> | The file path |

<a name="DropboxDatasource+load"></a>

### dropboxDatasource.load(credentials) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
Load an archive from the datasource

**Kind**: instance method of <code>[DropboxDatasource](#DropboxDatasource)</code>  
**Overrides:** <code>[load](#TextDatasource+load)</code>  
**Returns**: <code>[Promise.&lt;Archive&gt;](#Archive)</code> - A promise that resolves with an archive  

| Param | Type | Description |
| --- | --- | --- |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials for decryption |

<a name="DropboxDatasource+save"></a>

### dropboxDatasource.save(archive, credentials) ⇒ <code>Promise</code>
Save an archive using the datasource

**Kind**: instance method of <code>[DropboxDatasource](#DropboxDatasource)</code>  
**Overrides:** <code>[save](#TextDatasource+save)</code>  
**Returns**: <code>Promise</code> - A promise that resolves when saving has completed  

| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive to save |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials to save with |

<a name="DropboxDatasource+toObject"></a>

### dropboxDatasource.toObject() ⇒ <code>Object</code>
Output the datasource as an object

**Kind**: instance method of <code>[DropboxDatasource](#DropboxDatasource)</code>  
**Overrides:** <code>[toObject](#TextDatasource+toObject)</code>  
**Returns**: <code>Object</code> - An object describing the datasource  
<a name="TextDatasource+setContent"></a>

### dropboxDatasource.setContent(content) ⇒ <code>[TextDatasource](#TextDatasource)</code>
Set the text content

**Kind**: instance method of <code>[DropboxDatasource](#DropboxDatasource)</code>  
**Returns**: <code>[TextDatasource](#TextDatasource)</code> - Self  

| Param | Type | Description |
| --- | --- | --- |
| content | <code>String</code> | The encrypted text content |

<a name="TextDatasource+toString"></a>

### dropboxDatasource.toString() ⇒ <code>String</code>
Output the datasource configuration as a string

**Kind**: instance method of <code>[DropboxDatasource](#DropboxDatasource)</code>  
**Returns**: <code>String</code> - The string representation of the datasource  
<a name="Entry"></a>

## Entry
**Kind**: global class  

* [Entry](#Entry)
    * [new Entry(archive, remoteObj)](#new_Entry_new)
    * _instance_
        * [.delete()](#Entry+delete) ⇒ <code>Boolean</code>
        * [.deleteAttribute(attr)](#Entry+deleteAttribute) ⇒ <code>[Entry](#Entry)</code>
        * [.deleteMeta(property)](#Entry+deleteMeta) ⇒ <code>[Entry](#Entry)</code>
        * [.getAttribute([attributeName])](#Entry+getAttribute) ⇒ <code>String</code> &#124; <code>undefined</code> &#124; <code>Object</code>
        * [.getAttributes()](#Entry+getAttributes) ⇒ <code>Object</code>
        * [.getGroup()](#Entry+getGroup) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
        * [.getID()](#Entry+getID) ⇒ <code>String</code>
        * [.getMeta([property])](#Entry+getMeta) ⇒ <code>String</code> &#124; <code>undefined</code> &#124; <code>Object</code>
        * [.getProperty([property])](#Entry+getProperty) ⇒ <code>String</code> &#124; <code>undefined</code> &#124; <code>Object</code>
        * [.isInTrash()](#Entry+isInTrash) ⇒ <code>Boolean</code>
        * [.moveToGroup(group)](#Entry+moveToGroup) ⇒ <code>[Entry](#Entry)</code>
        * [.setAttribute(attributeName, value)](#Entry+setAttribute) ⇒ <code>[Entry](#Entry)</code>
        * [.setMeta(prop, [value])](#Entry+setMeta) ⇒ <code>[Entry](#Entry)</code>
        * [.setProperty(prop, [value])](#Entry+setProperty) ⇒ <code>[Entry](#Entry)</code>
        * [.toObject()](#Entry+toObject) ⇒ <code>Object</code>
        * [.toString()](#Entry+toString) ⇒ <code>String</code>
        * [._getArchive()](#Entry+_getArchive) ⇒ <code>[Archive](#Archive)</code>
        * [._getRemoteObject()](#Entry+_getRemoteObject) ⇒ <code>Object</code>
        * [._getWestley()](#Entry+_getWestley) ⇒ <code>[Westley](#Westley)</code>
    * _static_
        * [.createNew(archive, groupID)](#Entry.createNew) ⇒ <code>[Entry](#Entry)</code>

<a name="new_Entry_new"></a>

### new Entry(archive, remoteObj)
Managed entry class


| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The main archive instance |
| remoteObj | <code>Object</code> | The remote object reference |

<a name="Entry+delete"></a>

### entry.delete() ⇒ <code>Boolean</code>
Delete the entry - either trashes the entry, or removes it completely.
If the entry is in the trash already, it is removed (including if there is no
   trash group). If the entry is in a normal group and a trash group exists, it
 is moved there instead of being deleted.

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>Boolean</code> - Whether or not the item was deleted  
**See**

- moveToGroup
- Archive.getTrashGroup

<a name="Entry+deleteAttribute"></a>

### entry.deleteAttribute(attr) ⇒ <code>[Entry](#Entry)</code>
Delete an attribute

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>[Entry](#Entry)</code> - Self  
**Throws**:

- <code>Error</code> Throws if the attribute doesn't exist, or cannot be deleted


| Param | Type | Description |
| --- | --- | --- |
| attr | <code>String</code> | The attribute name |

<a name="Entry+deleteMeta"></a>

### entry.deleteMeta(property) ⇒ <code>[Entry](#Entry)</code>
Delete a meta item

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>[Entry](#Entry)</code> - Self  
**Throws**:

- <code>Error</code> Throws if property doesn't exist, or cannot be deleted


| Param | Type | Description |
| --- | --- | --- |
| property | <code>String</code> | The meta property to delete |

<a name="Entry+getAttribute"></a>

### entry.getAttribute([attributeName]) ⇒ <code>String</code> &#124; <code>undefined</code> &#124; <code>Object</code>
Get an attribute
If no attribute name is specified, an object with all attributes and their
values is returned.

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>String</code> &#124; <code>undefined</code> &#124; <code>Object</code> - The attribute value or an object
 containing all attribute keys and their values if no attribute name
 is provided  

| Param | Type | Description |
| --- | --- | --- |
| [attributeName] | <code>String</code> | The name of the attribute to fetch |

<a name="Entry+getAttributes"></a>

### entry.getAttributes() ⇒ <code>Object</code>
Get all attributes

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>Object</code> - Attributes object  
<a name="Entry+getGroup"></a>

### entry.getGroup() ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
Get the containing group for the entry

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>[Group](#Group)</code> &#124; <code>null</code> - The parent group  
<a name="Entry+getID"></a>

### entry.getID() ⇒ <code>String</code>
Get the entry ID

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>String</code> - The entry's ID  
<a name="Entry+getMeta"></a>

### entry.getMeta([property]) ⇒ <code>String</code> &#124; <code>undefined</code> &#124; <code>Object</code>
Get a meta value
If no meta name is specified, an object with all meta keys and their
values is returned.

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>String</code> &#124; <code>undefined</code> &#124; <code>Object</code> - The meta value or an object
 containing all meta keys and values if no meta name specified  

| Param | Type | Description |
| --- | --- | --- |
| [property] | <code>String</code> | The name of the meta property |

<a name="Entry+getProperty"></a>

### entry.getProperty([property]) ⇒ <code>String</code> &#124; <code>undefined</code> &#124; <code>Object</code>
Get a property value
If no property name is specified, an object with all properties and their
values is returned.

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>String</code> &#124; <code>undefined</code> &#124; <code>Object</code> - The property value or an object with all
 values if no property specified  

| Param | Type | Description |
| --- | --- | --- |
| [property] | <code>String</code> | The name of the property to fetch |

<a name="Entry+isInTrash"></a>

### entry.isInTrash() ⇒ <code>Boolean</code>
Check if the entry is in the trash

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>Boolean</code> - Whether or not the entry is in the trash  
<a name="Entry+moveToGroup"></a>

### entry.moveToGroup(group) ⇒ <code>[Entry](#Entry)</code>
Move the entry to another group

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>[Entry](#Entry)</code> - Returns self  
**Params**: <code>[Group](#Group)</code> group The target group  

| Param | Type | Description |
| --- | --- | --- |
| group | <code>[Group](#Group)</code> | The target group |

<a name="Entry+setAttribute"></a>

### entry.setAttribute(attributeName, value) ⇒ <code>[Entry](#Entry)</code>
Set an attribute on the entry

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>[Entry](#Entry)</code> - Returns self  

| Param | Type | Description |
| --- | --- | --- |
| attributeName | <code>String</code> | The name of the attribute |
| value | <code>String</code> | The value to set |

<a name="Entry+setMeta"></a>

### entry.setMeta(prop, [value]) ⇒ <code>[Entry](#Entry)</code>
Set a meta value on the entry

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>[Entry](#Entry)</code> - Returns self  

| Param | Type | Description |
| --- | --- | --- |
| prop | <code>String</code> | The meta name |
| [value] | <code>String</code> | The value to set |

<a name="Entry+setProperty"></a>

### entry.setProperty(prop, [value]) ⇒ <code>[Entry](#Entry)</code>
Set a property on the entry

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>[Entry](#Entry)</code> - Returns self  

| Param | Type | Description |
| --- | --- | --- |
| prop | <code>String</code> | The property name |
| [value] | <code>String</code> | The property value |

<a name="Entry+toObject"></a>

### entry.toObject() ⇒ <code>Object</code>
Export entry to object

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>Object</code> - The entry in object-form  
<a name="Entry+toString"></a>

### entry.toString() ⇒ <code>String</code>
toString override

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>String</code> - The string representation of the Entry  
<a name="Entry+_getArchive"></a>

### entry._getArchive() ⇒ <code>[Archive](#Archive)</code>
Get the archive reference

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>[Archive](#Archive)</code> - The Archive reference  
<a name="Entry+_getRemoteObject"></a>

### entry._getRemoteObject() ⇒ <code>Object</code>
Get the remote object that mirrors the data represented here

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>Object</code> - The remote object (in-memory copy)  
<a name="Entry+_getWestley"></a>

### entry._getWestley() ⇒ <code>[Westley](#Westley)</code>
Get the Westley reference

**Kind**: instance method of <code>[Entry](#Entry)</code>  
**Returns**: <code>[Westley](#Westley)</code> - The internal Westley reference  
<a name="Entry.createNew"></a>

### Entry.createNew(archive, groupID) ⇒ <code>[Entry](#Entry)</code>
Create a new entry

**Kind**: static method of <code>[Entry](#Entry)</code>  
**Returns**: <code>[Entry](#Entry)</code> - The new entry  
**Throws**:

- <code>Error</code> Throws if the target group doesn't exist
- <code>Error</code> Throws if the target group is the trash group,
     or if the target group is in the trash


| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive |
| groupID | <code>string</code> | The ID of the target group |

<a name="EntryFinder"></a>

## EntryFinder
Entry searching class

**Kind**: global class  

* [EntryFinder](#EntryFinder)
    * [new EntryFinder(target)](#new_EntryFinder_new)
    * [.items](#EntryFinder+items) : <code>[Array.&lt;EntrySearchInfo&gt;](#EntrySearchInfo)</code>
    * [.lastResult](#EntryFinder+lastResult) : <code>[Array.&lt;EntrySearchInfo&gt;](#EntrySearchInfo)</code>
    * [.initSearcher()](#EntryFinder+initSearcher)
    * [.search(term)](#EntryFinder+search) ⇒ <code>[Array.&lt;EntrySearchInfo&gt;](#EntrySearchInfo)</code>

<a name="new_EntryFinder_new"></a>

### new EntryFinder(target)

| Param | Type | Description |
| --- | --- | --- |
| target | <code>[Array.&lt;Archive&gt;](#Archive)</code> &#124; <code>[Archive](#Archive)</code> | The archive or archives to search |

<a name="EntryFinder+items"></a>

### entryFinder.items : <code>[Array.&lt;EntrySearchInfo&gt;](#EntrySearchInfo)</code>
All items available for searching

**Kind**: instance property of <code>[EntryFinder](#EntryFinder)</code>  
<a name="EntryFinder+lastResult"></a>

### entryFinder.lastResult : <code>[Array.&lt;EntrySearchInfo&gt;](#EntrySearchInfo)</code>
The last result

**Kind**: instance property of <code>[EntryFinder](#EntryFinder)</code>  
<a name="EntryFinder+initSearcher"></a>

### entryFinder.initSearcher()
Initialise the searching mechanism

**Kind**: instance method of <code>[EntryFinder](#EntryFinder)</code>  
<a name="EntryFinder+search"></a>

### entryFinder.search(term) ⇒ <code>[Array.&lt;EntrySearchInfo&gt;](#EntrySearchInfo)</code>
Search and get results

**Kind**: instance method of <code>[EntryFinder](#EntryFinder)</code>  
**Returns**: <code>[Array.&lt;EntrySearchInfo&gt;](#EntrySearchInfo)</code> - The results  

| Param | Type | Description |
| --- | --- | --- |
| term | <code>String</code> | The search term |

<a name="FileDatasource"></a>

## FileDatasource ⇐ <code>[TextDatasource](#TextDatasource)</code>
**Kind**: global class  
**Extends:** <code>[TextDatasource](#TextDatasource)</code>  

* [FileDatasource](#FileDatasource) ⇐ <code>[TextDatasource](#TextDatasource)</code>
    * [new FileDatasource()](#new_FileDatasource_new)
    * [new FileDatasource(filename)](#new_FileDatasource_new)
    * [.getArchivePath()](#FileDatasource+getArchivePath) ⇒ <code>String</code>
    * [.load(credentials)](#FileDatasource+load) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
    * [.save(archive, credentials)](#FileDatasource+save) ⇒ <code>Promise</code>
    * [.toObject()](#FileDatasource+toObject) ⇒ <code>Object</code>
    * [.setContent(content)](#TextDatasource+setContent) ⇒ <code>[TextDatasource](#TextDatasource)</code>
    * [.toString()](#TextDatasource+toString) ⇒ <code>String</code>

<a name="new_FileDatasource_new"></a>

### new FileDatasource()
File datasource for loading and saving files

<a name="new_FileDatasource_new"></a>

### new FileDatasource(filename)
Constructor for the file datasource


| Param | Type | Description |
| --- | --- | --- |
| filename | <code>string</code> | The filename to load and save |

<a name="FileDatasource+getArchivePath"></a>

### fileDatasource.getArchivePath() ⇒ <code>String</code>
Get the path of the archive

**Kind**: instance method of <code>[FileDatasource](#FileDatasource)</code>  
**Returns**: <code>String</code> - The file path  
<a name="FileDatasource+load"></a>

### fileDatasource.load(credentials) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
Load from the filename specified in the constructor using a password

**Kind**: instance method of <code>[FileDatasource](#FileDatasource)</code>  
**Overrides:** <code>[load](#TextDatasource+load)</code>  
**Returns**: <code>[Promise.&lt;Archive&gt;](#Archive)</code> - A promise resolving with the opened archive  

| Param | Type | Description |
| --- | --- | --- |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials for decryption |

<a name="FileDatasource+save"></a>

### fileDatasource.save(archive, credentials) ⇒ <code>Promise</code>
Save an archive to a file using a password for encryption

**Kind**: instance method of <code>[FileDatasource](#FileDatasource)</code>  
**Overrides:** <code>[save](#TextDatasource+save)</code>  
**Returns**: <code>Promise</code> - A promise that resolves when saving is complete  

| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive to save |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials to save with |

<a name="FileDatasource+toObject"></a>

### fileDatasource.toObject() ⇒ <code>Object</code>
Output the datasource as an object

**Kind**: instance method of <code>[FileDatasource](#FileDatasource)</code>  
**Overrides:** <code>[toObject](#TextDatasource+toObject)</code>  
**Returns**: <code>Object</code> - An object describing the datasource  
<a name="TextDatasource+setContent"></a>

### fileDatasource.setContent(content) ⇒ <code>[TextDatasource](#TextDatasource)</code>
Set the text content

**Kind**: instance method of <code>[FileDatasource](#FileDatasource)</code>  
**Returns**: <code>[TextDatasource](#TextDatasource)</code> - Self  

| Param | Type | Description |
| --- | --- | --- |
| content | <code>String</code> | The encrypted text content |

<a name="TextDatasource+toString"></a>

### fileDatasource.toString() ⇒ <code>String</code>
Output the datasource configuration as a string

**Kind**: instance method of <code>[FileDatasource](#FileDatasource)</code>  
**Returns**: <code>String</code> - The string representation of the datasource  
<a name="FileDatasource"></a>

## FileDatasource
**Kind**: global class  

* [FileDatasource](#FileDatasource)
    * [new FileDatasource()](#new_FileDatasource_new)
    * [new FileDatasource(filename)](#new_FileDatasource_new)
    * [.getArchivePath()](#FileDatasource+getArchivePath) ⇒ <code>String</code>
    * [.load(credentials)](#FileDatasource+load) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
    * [.save(archive, credentials)](#FileDatasource+save) ⇒ <code>Promise</code>
    * [.toObject()](#FileDatasource+toObject) ⇒ <code>Object</code>
    * [.setContent(content)](#TextDatasource+setContent) ⇒ <code>[TextDatasource](#TextDatasource)</code>
    * [.toString()](#TextDatasource+toString) ⇒ <code>String</code>

<a name="new_FileDatasource_new"></a>

### new FileDatasource()
File datasource for loading and saving files

<a name="new_FileDatasource_new"></a>

### new FileDatasource(filename)
Constructor for the file datasource


| Param | Type | Description |
| --- | --- | --- |
| filename | <code>string</code> | The filename to load and save |

<a name="FileDatasource+getArchivePath"></a>

### fileDatasource.getArchivePath() ⇒ <code>String</code>
Get the path of the archive

**Kind**: instance method of <code>[FileDatasource](#FileDatasource)</code>  
**Returns**: <code>String</code> - The file path  
<a name="FileDatasource+load"></a>

### fileDatasource.load(credentials) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
Load from the filename specified in the constructor using a password

**Kind**: instance method of <code>[FileDatasource](#FileDatasource)</code>  
**Overrides:** <code>[load](#TextDatasource+load)</code>  
**Returns**: <code>[Promise.&lt;Archive&gt;](#Archive)</code> - A promise resolving with the opened archive  

| Param | Type | Description |
| --- | --- | --- |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials for decryption |

<a name="FileDatasource+save"></a>

### fileDatasource.save(archive, credentials) ⇒ <code>Promise</code>
Save an archive to a file using a password for encryption

**Kind**: instance method of <code>[FileDatasource](#FileDatasource)</code>  
**Overrides:** <code>[save](#TextDatasource+save)</code>  
**Returns**: <code>Promise</code> - A promise that resolves when saving is complete  

| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive to save |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials to save with |

<a name="FileDatasource+toObject"></a>

### fileDatasource.toObject() ⇒ <code>Object</code>
Output the datasource as an object

**Kind**: instance method of <code>[FileDatasource](#FileDatasource)</code>  
**Overrides:** <code>[toObject](#TextDatasource+toObject)</code>  
**Returns**: <code>Object</code> - An object describing the datasource  
<a name="TextDatasource+setContent"></a>

### fileDatasource.setContent(content) ⇒ <code>[TextDatasource](#TextDatasource)</code>
Set the text content

**Kind**: instance method of <code>[FileDatasource](#FileDatasource)</code>  
**Returns**: <code>[TextDatasource](#TextDatasource)</code> - Self  

| Param | Type | Description |
| --- | --- | --- |
| content | <code>String</code> | The encrypted text content |

<a name="TextDatasource+toString"></a>

### fileDatasource.toString() ⇒ <code>String</code>
Output the datasource configuration as a string

**Kind**: instance method of <code>[FileDatasource](#FileDatasource)</code>  
**Returns**: <code>String</code> - The string representation of the datasource  
<a name="Flattener"></a>

## Flattener
**Kind**: global class  

* [Flattener](#Flattener)
    * [new Flattener(westley)](#new_Flattener_new)
    * [.canBeFlattened()](#Flattener+canBeFlattened) ⇒ <code>Boolean</code>
    * [.flatten([force])](#Flattener+flatten) ⇒ <code>Boolean</code>
    * [.getPreservationCount()](#Flattener+getPreservationCount) ⇒ <code>Number</code>

<a name="new_Flattener_new"></a>

### new Flattener(westley)
Flatten archives


| Param | Type | Description |
| --- | --- | --- |
| westley | <code>[Westley](#Westley)</code> | The Westley instance |

<a name="Flattener+canBeFlattened"></a>

### flattener.canBeFlattened() ⇒ <code>Boolean</code>
Check if the dataset can be flattened

**Kind**: instance method of <code>[Flattener](#Flattener)</code>  
**Returns**: <code>Boolean</code> - True if it can be flattened  
**Access:** public  
<a name="Flattener+flatten"></a>

### flattener.flatten([force]) ⇒ <code>Boolean</code>
Flatten a dataset

**Kind**: instance method of <code>[Flattener](#Flattener)</code>  
**Returns**: <code>Boolean</code> - True if flattening occurred, false otherwise  
**Access:** public  

| Param | Type | Description |
| --- | --- | --- |
| [force] | <code>Boolean</code> | Force flattening even if it is detected to be unnecessary |

<a name="Flattener+getPreservationCount"></a>

### flattener.getPreservationCount() ⇒ <code>Number</code>
Get the number of lines to preserve by default

**Kind**: instance method of <code>[Flattener](#Flattener)</code>  
**Returns**: <code>Number</code> - The number of lines  
**Access:** public  
**See**: PRESERVE_LAST_LINES  
<a name="Group"></a>

## Group
**Kind**: global class  
**Mixes**: <code>[GroupCollection](#GroupCollection)</code>, <code>[EntryCollection](#EntryCollection)</code>  

* [Group](#Group)
    * [new Group()](#new_Group_new)
    * [new Group(archive, remoteObj)](#new_Group_new)
    * _instance_
        * [.type](#Group+type) : <code>String</code>
        * [.findGroupByID](#Group+findGroupByID) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
        * [.findGroupsByTitle](#Group+findGroupsByTitle) ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
        * [.findEntriesByMeta](#Group+findEntriesByMeta) ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
        * [.findEntriesByProperty](#Group+findEntriesByProperty) ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
        * [.createEntry([title])](#Group+createEntry) ⇒ <code>[Entry](#Entry)</code>
        * [.createGroup([title])](#Group+createGroup) ⇒ <code>[Group](#Group)</code>
        * [.delete([skipTrash])](#Group+delete) ⇒ <code>Boolean</code>
        * [.deleteAttribute(attr)](#Group+deleteAttribute) ⇒ <code>[Group](#Group)</code>
        * [.getAttribute(attributeName)](#Group+getAttribute) ⇒ <code>string</code> &#124; <code>undefined</code>
        * [.getAttributes()](#Group+getAttributes) ⇒ <code>Object</code>
        * [.getEntries()](#Group+getEntries) ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
        * [.getGroup()](#Group+getGroup) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
        * ~~[.getGroupByID(groupID)](#Group+getGroupByID) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>~~
        * [.getGroups()](#Group+getGroups) ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
        * [.getID()](#Group+getID) ⇒ <code>string</code>
        * [.getTitle()](#Group+getTitle) ⇒ <code>string</code>
        * [.isForeign()](#Group+isForeign) ⇒ <code>Boolean</code>
        * [.isInTrash()](#Group+isInTrash) ⇒ <code>Boolean</code>
        * [.isShared()](#Group+isShared) ⇒ <code>Boolean</code>
        * [.isTrash()](#Group+isTrash) ⇒ <code>Boolean</code>
        * [.moveTo(target)](#Group+moveTo) ⇒ <code>[Group](#Group)</code>
        * ~~[.moveToGroup(group)](#Group+moveToGroup) ⇒ <code>[Group](#Group)</code>~~
        * [.setAttribute(attributeName, value)](#Group+setAttribute) ⇒ <code>[Group](#Group)</code>
        * [.setTitle(title)](#Group+setTitle) ⇒ <code>[Group](#Group)</code>
        * [.toObject(outputFlags)](#Group+toObject) ⇒ <code>Object</code>
        * [.toString(outputFlags)](#Group+toString) ⇒ <code>string</code>
        * [._getArchive()](#Group+_getArchive) ⇒ <code>[Archive](#Archive)</code>
        * [._getRemoteObject()](#Group+_getRemoteObject) ⇒ <code>Object</code>
        * [._getWestley()](#Group+_getWestley) ⇒ <code>[Westley](#Westley)</code>
        * [.inst.findEntryByID(id)](#Group+findEntryByID) ⇒ <code>null</code> &#124; <code>[Entry](#Entry)</code>
    * _static_
        * [.Attributes](#Group.Attributes) : <code>enum</code>
        * [.OutputFlag](#Group.OutputFlag) : <code>enum</code>
        * [.createNew(archive, [parentID])](#Group.createNew) ⇒ <code>[Group](#Group)</code>

<a name="new_Group_new"></a>

### new Group()
Buttercup Group

<a name="new_Group_new"></a>

### new Group(archive, remoteObj)
Managed group class


| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive instance |
| remoteObj | <code>Object</code> | The remote object reference |

<a name="Group+type"></a>

### group.type : <code>String</code>
Get the instance type

**Kind**: instance property of <code>[Group](#Group)</code>  
<a name="Group+findGroupByID"></a>

### group.findGroupByID ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
Find a group by its ID

**Kind**: instance property of <code>[Group](#Group)</code>  
**Mixes**: <code>[findGroupByID](#GroupCollection.findGroupByID)</code>  
**Returns**: <code>[Group](#Group)</code> &#124; <code>null</code> - The group or null if not found  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The group ID to search for |

<a name="Group+findGroupsByTitle"></a>

### group.findGroupsByTitle ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
Find groups by their title

**Kind**: instance property of <code>[Group](#Group)</code>  
**Mixes**: <code>[findGroupsByTitle](#GroupCollection.findGroupsByTitle)</code>  
**Returns**: <code>[Array.&lt;Group&gt;](#Group)</code> - An array of groups  

| Param | Type | Description |
| --- | --- | --- |
| title | <code>String</code> &#124; <code>RegExp</code> | The group title |

<a name="Group+findEntriesByMeta"></a>

### group.findEntriesByMeta ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
Find entries that match a certain meta property

**Kind**: instance property of <code>[Group](#Group)</code>  
**Mixes**: <code>[findEntriesByMeta](#EntryCollection.findEntriesByMeta)</code>  
**Returns**: <code>[Array.&lt;Entry&gt;](#Entry)</code> - An array of found entries  

| Param | Type | Description |
| --- | --- | --- |
| metaName | <code>String</code> | The meta property to search for |
| value | <code>RegExp</code> &#124; <code>string</code> | The value to search for |

<a name="Group+findEntriesByProperty"></a>

### group.findEntriesByProperty ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
Find all entries that match a certain property

**Kind**: instance property of <code>[Group](#Group)</code>  
**Mixes**: <code>[findEntriesByProperty](#EntryCollection.findEntriesByProperty)</code>  
**Returns**: <code>[Array.&lt;Entry&gt;](#Entry)</code> - An array of found extries  

| Param | Type | Description |
| --- | --- | --- |
| property | <code>string</code> | The property to search with |
| value | <code>RegExp</code> &#124; <code>string</code> | The value to search for |

<a name="Group+createEntry"></a>

### group.createEntry([title]) ⇒ <code>[Entry](#Entry)</code>
Create a new entry with a title

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Entry](#Entry)</code> - The new entry  

| Param | Type | Description |
| --- | --- | --- |
| [title] | <code>string</code> | The title of the new entry |

<a name="Group+createGroup"></a>

### group.createGroup([title]) ⇒ <code>[Group](#Group)</code>
Create a child group

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - The new child group  

| Param | Type | Description |
| --- | --- | --- |
| [title] | <code>string</code> | Optionally set a title |

<a name="Group+delete"></a>

### group.delete([skipTrash]) ⇒ <code>Boolean</code>
Delete the group
If there is a trash group available, the group is moved there. If the group
is already in the trash, it is deleted permanently.

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Boolean</code> - True when deleted, false when moved to trash  

| Param | Type | Description |
| --- | --- | --- |
| [skipTrash] | <code>Boolean</code> | Skip the trash |

<a name="Group+deleteAttribute"></a>

### group.deleteAttribute(attr) ⇒ <code>[Group](#Group)</code>
Delete an attribute

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - Returns self  

| Param | Type | Description |
| --- | --- | --- |
| attr | <code>string</code> | The name of the attribute |

<a name="Group+getAttribute"></a>

### group.getAttribute(attributeName) ⇒ <code>string</code> &#124; <code>undefined</code>
Get an attribute

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>string</code> &#124; <code>undefined</code> - Returns the attribute or undefined if not found  

| Param | Type | Description |
| --- | --- | --- |
| attributeName | <code>string</code> | The name of the attribute |

<a name="Group+getAttributes"></a>

### group.getAttributes() ⇒ <code>Object</code>
Get all attributes

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Object</code> - Attributes object  
<a name="Group+getEntries"></a>

### group.getEntries() ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
Get the entries within the group

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Array.&lt;Entry&gt;](#Entry)</code> - An array of entries  
<a name="Group+getGroup"></a>

### group.getGroup() ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
Get the parent group

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> &#124; <code>null</code> - Returns the parent group instance or null if the parent
 is the archive  
**Throws**:

- <code>Error</code> Throws if no parent could be found (detached)

<a name="Group+getGroupByID"></a>

### ~~group.getGroupByID(groupID) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>~~
***Deprecated***

Get a child group (deep) by its ID

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> &#124; <code>null</code> - The found group or null  
**See**: findGroupByID  

| Param | Type | Description |
| --- | --- | --- |
| groupID | <code>String</code> | The ID of the group to get |

<a name="Group+getGroups"></a>

### group.getGroups() ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
Get the groups within the group

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Array.&lt;Group&gt;](#Group)</code> - An array of child groups  
<a name="Group+getID"></a>

### group.getID() ⇒ <code>string</code>
Get the group ID

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>string</code> - The ID of the group  
<a name="Group+getTitle"></a>

### group.getTitle() ⇒ <code>string</code>
Get the group title

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>string</code> - The title of the group  
<a name="Group+isForeign"></a>

### group.isForeign() ⇒ <code>Boolean</code>
Check if the group is foreign (from another archive)

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Boolean</code> - True if it is foreign  
<a name="Group+isInTrash"></a>

### group.isInTrash() ⇒ <code>Boolean</code>
Check if the group is in the trash

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Boolean</code> - Whether or not the group is within the trash group  
<a name="Group+isShared"></a>

### group.isShared() ⇒ <code>Boolean</code>
Check if the group is shared

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Boolean</code> - True if the group is a shared group  
<a name="Group+isTrash"></a>

### group.isTrash() ⇒ <code>Boolean</code>
Check if the group is used for trash

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Boolean</code> - Whether or not the group is the trash group  
<a name="Group+moveTo"></a>

### group.moveTo(target) ⇒ <code>[Group](#Group)</code>
Move the group to another group or archive

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - Self  

| Param | Type | Description |
| --- | --- | --- |
| target | <code>[Group](#Group)</code> &#124; <code>[Archive](#Archive)</code> | The destination Group or Archive instance |

<a name="Group+moveToGroup"></a>

### ~~group.moveToGroup(group) ⇒ <code>[Group](#Group)</code>~~
***Deprecated***

Move the group into another

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - Returns self  
**See**: moveTo  

| Param | Type | Description |
| --- | --- | --- |
| group | <code>[Group](#Group)</code> | The target group (new parent) |

<a name="Group+setAttribute"></a>

### group.setAttribute(attributeName, value) ⇒ <code>[Group](#Group)</code>
Set an attribute

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - Returns self  

| Param | Type | Description |
| --- | --- | --- |
| attributeName | <code>string</code> | The name of the attribute |
| value | <code>string</code> | The value to set |

<a name="Group+setTitle"></a>

### group.setTitle(title) ⇒ <code>[Group](#Group)</code>
Set the group title

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - Returns self  

| Param | Type | Description |
| --- | --- | --- |
| title | <code>string</code> | The title of the group |

<a name="Group+toObject"></a>

### group.toObject(outputFlags) ⇒ <code>Object</code>
Export group to object

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Object</code> - The group, in raw object form  

| Param | Type | Description |
| --- | --- | --- |
| outputFlags | <code>Number</code> | Bitwise options for outputting entries and child groups |

**Example**  
```js
// output defaults (entries and sub groups)
     group.toObject()
```
**Example**  
```js
// output only entries
     group.toObject(Group.OutputFlag.Entries)
```
**Example**  
```js
// output only the group info
     group.toObject(Group.OutputFlag.OnlyGroup)
```
<a name="Group+toString"></a>

### group.toString(outputFlags) ⇒ <code>string</code>
Export the group to a JSON string

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>string</code> - The group (and entries) in JSON string format  
**See**: toObject  

| Param | Type | Description |
| --- | --- | --- |
| outputFlags | <code>Number</code> | Output configuration flags to pass to `toObject` |

<a name="Group+_getArchive"></a>

### group._getArchive() ⇒ <code>[Archive](#Archive)</code>
Get the archive instance reference

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Archive](#Archive)</code> - The archive instance  
**Access:** protected  
<a name="Group+_getRemoteObject"></a>

### group._getRemoteObject() ⇒ <code>Object</code>
Get the remotely-managed object (group)

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Object</code> - The object instance for the group  
**Access:** protected  
<a name="Group+_getWestley"></a>

### group._getWestley() ⇒ <code>[Westley](#Westley)</code>
Get the delta managing instance for the archive

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Westley](#Westley)</code> - The internal Westley object  
**Access:** protected  
<a name="Group+findEntryByID"></a>

### group.inst.findEntryByID(id) ⇒ <code>null</code> &#124; <code>[Entry](#Entry)</code>
Find an entry by its ID

**Kind**: instance method of <code>[Group](#Group)</code>  
**Mixes**: <code>[inst.findEntryByID](#EntryCollection.inst.findEntryByID)</code>  
**Returns**: <code>null</code> &#124; <code>[Entry](#Entry)</code> - Null if not found, or the Entry instance  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The ID to search for |

<a name="Group.Attributes"></a>

### Group.Attributes : <code>enum</code>
Group attribute names

**Kind**: static enum property of <code>[Group](#Group)</code>  
<a name="Group.OutputFlag"></a>

### Group.OutputFlag : <code>enum</code>
Bitwise output flags for `toObject` and `toString`

**Kind**: static enum property of <code>[Group](#Group)</code>  
**See**

- toObject
- toString

<a name="Group.createNew"></a>

### Group.createNew(archive, [parentID]) ⇒ <code>[Group](#Group)</code>
Create a new Group with a delta-manager and parent group ID

**Kind**: static method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - A new group  
**Throws**:

- <code>Error</code> Throws if the target group doesn't exist
- <code>Error</code> Throws if the target group is the trash group,
     or if the target group is within the trash group


| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive to create the group in |
| [parentID] | <code>string</code> | The parent group ID (default is root) |

<a name="Group"></a>

## Group
**Kind**: global class  

* [Group](#Group)
    * [new Group()](#new_Group_new)
    * [new Group(archive, remoteObj)](#new_Group_new)
    * _instance_
        * [.type](#Group+type) : <code>String</code>
        * [.findGroupByID](#Group+findGroupByID) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
        * [.findGroupsByTitle](#Group+findGroupsByTitle) ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
        * [.findEntriesByMeta](#Group+findEntriesByMeta) ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
        * [.findEntriesByProperty](#Group+findEntriesByProperty) ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
        * [.createEntry([title])](#Group+createEntry) ⇒ <code>[Entry](#Entry)</code>
        * [.createGroup([title])](#Group+createGroup) ⇒ <code>[Group](#Group)</code>
        * [.delete([skipTrash])](#Group+delete) ⇒ <code>Boolean</code>
        * [.deleteAttribute(attr)](#Group+deleteAttribute) ⇒ <code>[Group](#Group)</code>
        * [.getAttribute(attributeName)](#Group+getAttribute) ⇒ <code>string</code> &#124; <code>undefined</code>
        * [.getAttributes()](#Group+getAttributes) ⇒ <code>Object</code>
        * [.getEntries()](#Group+getEntries) ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
        * [.getGroup()](#Group+getGroup) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
        * ~~[.getGroupByID(groupID)](#Group+getGroupByID) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>~~
        * [.getGroups()](#Group+getGroups) ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
        * [.getID()](#Group+getID) ⇒ <code>string</code>
        * [.getTitle()](#Group+getTitle) ⇒ <code>string</code>
        * [.isForeign()](#Group+isForeign) ⇒ <code>Boolean</code>
        * [.isInTrash()](#Group+isInTrash) ⇒ <code>Boolean</code>
        * [.isShared()](#Group+isShared) ⇒ <code>Boolean</code>
        * [.isTrash()](#Group+isTrash) ⇒ <code>Boolean</code>
        * [.moveTo(target)](#Group+moveTo) ⇒ <code>[Group](#Group)</code>
        * ~~[.moveToGroup(group)](#Group+moveToGroup) ⇒ <code>[Group](#Group)</code>~~
        * [.setAttribute(attributeName, value)](#Group+setAttribute) ⇒ <code>[Group](#Group)</code>
        * [.setTitle(title)](#Group+setTitle) ⇒ <code>[Group](#Group)</code>
        * [.toObject(outputFlags)](#Group+toObject) ⇒ <code>Object</code>
        * [.toString(outputFlags)](#Group+toString) ⇒ <code>string</code>
        * [._getArchive()](#Group+_getArchive) ⇒ <code>[Archive](#Archive)</code>
        * [._getRemoteObject()](#Group+_getRemoteObject) ⇒ <code>Object</code>
        * [._getWestley()](#Group+_getWestley) ⇒ <code>[Westley](#Westley)</code>
        * [.inst.findEntryByID(id)](#Group+findEntryByID) ⇒ <code>null</code> &#124; <code>[Entry](#Entry)</code>
    * _static_
        * [.Attributes](#Group.Attributes) : <code>enum</code>
        * [.OutputFlag](#Group.OutputFlag) : <code>enum</code>
        * [.createNew(archive, [parentID])](#Group.createNew) ⇒ <code>[Group](#Group)</code>

<a name="new_Group_new"></a>

### new Group()
Buttercup Group

<a name="new_Group_new"></a>

### new Group(archive, remoteObj)
Managed group class


| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive instance |
| remoteObj | <code>Object</code> | The remote object reference |

<a name="Group+type"></a>

### group.type : <code>String</code>
Get the instance type

**Kind**: instance property of <code>[Group](#Group)</code>  
<a name="Group+findGroupByID"></a>

### group.findGroupByID ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
Find a group by its ID

**Kind**: instance property of <code>[Group](#Group)</code>  
**Mixes**: <code>[findGroupByID](#GroupCollection.findGroupByID)</code>  
**Returns**: <code>[Group](#Group)</code> &#124; <code>null</code> - The group or null if not found  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The group ID to search for |

<a name="Group+findGroupsByTitle"></a>

### group.findGroupsByTitle ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
Find groups by their title

**Kind**: instance property of <code>[Group](#Group)</code>  
**Mixes**: <code>[findGroupsByTitle](#GroupCollection.findGroupsByTitle)</code>  
**Returns**: <code>[Array.&lt;Group&gt;](#Group)</code> - An array of groups  

| Param | Type | Description |
| --- | --- | --- |
| title | <code>String</code> &#124; <code>RegExp</code> | The group title |

<a name="Group+findEntriesByMeta"></a>

### group.findEntriesByMeta ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
Find entries that match a certain meta property

**Kind**: instance property of <code>[Group](#Group)</code>  
**Mixes**: <code>[findEntriesByMeta](#EntryCollection.findEntriesByMeta)</code>  
**Returns**: <code>[Array.&lt;Entry&gt;](#Entry)</code> - An array of found entries  

| Param | Type | Description |
| --- | --- | --- |
| metaName | <code>String</code> | The meta property to search for |
| value | <code>RegExp</code> &#124; <code>string</code> | The value to search for |

<a name="Group+findEntriesByProperty"></a>

### group.findEntriesByProperty ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
Find all entries that match a certain property

**Kind**: instance property of <code>[Group](#Group)</code>  
**Mixes**: <code>[findEntriesByProperty](#EntryCollection.findEntriesByProperty)</code>  
**Returns**: <code>[Array.&lt;Entry&gt;](#Entry)</code> - An array of found extries  

| Param | Type | Description |
| --- | --- | --- |
| property | <code>string</code> | The property to search with |
| value | <code>RegExp</code> &#124; <code>string</code> | The value to search for |

<a name="Group+createEntry"></a>

### group.createEntry([title]) ⇒ <code>[Entry](#Entry)</code>
Create a new entry with a title

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Entry](#Entry)</code> - The new entry  

| Param | Type | Description |
| --- | --- | --- |
| [title] | <code>string</code> | The title of the new entry |

<a name="Group+createGroup"></a>

### group.createGroup([title]) ⇒ <code>[Group](#Group)</code>
Create a child group

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - The new child group  

| Param | Type | Description |
| --- | --- | --- |
| [title] | <code>string</code> | Optionally set a title |

<a name="Group+delete"></a>

### group.delete([skipTrash]) ⇒ <code>Boolean</code>
Delete the group
If there is a trash group available, the group is moved there. If the group
is already in the trash, it is deleted permanently.

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Boolean</code> - True when deleted, false when moved to trash  

| Param | Type | Description |
| --- | --- | --- |
| [skipTrash] | <code>Boolean</code> | Skip the trash |

<a name="Group+deleteAttribute"></a>

### group.deleteAttribute(attr) ⇒ <code>[Group](#Group)</code>
Delete an attribute

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - Returns self  

| Param | Type | Description |
| --- | --- | --- |
| attr | <code>string</code> | The name of the attribute |

<a name="Group+getAttribute"></a>

### group.getAttribute(attributeName) ⇒ <code>string</code> &#124; <code>undefined</code>
Get an attribute

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>string</code> &#124; <code>undefined</code> - Returns the attribute or undefined if not found  

| Param | Type | Description |
| --- | --- | --- |
| attributeName | <code>string</code> | The name of the attribute |

<a name="Group+getAttributes"></a>

### group.getAttributes() ⇒ <code>Object</code>
Get all attributes

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Object</code> - Attributes object  
<a name="Group+getEntries"></a>

### group.getEntries() ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
Get the entries within the group

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Array.&lt;Entry&gt;](#Entry)</code> - An array of entries  
<a name="Group+getGroup"></a>

### group.getGroup() ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
Get the parent group

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> &#124; <code>null</code> - Returns the parent group instance or null if the parent
 is the archive  
**Throws**:

- <code>Error</code> Throws if no parent could be found (detached)

<a name="Group+getGroupByID"></a>

### ~~group.getGroupByID(groupID) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>~~
***Deprecated***

Get a child group (deep) by its ID

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> &#124; <code>null</code> - The found group or null  
**See**: findGroupByID  

| Param | Type | Description |
| --- | --- | --- |
| groupID | <code>String</code> | The ID of the group to get |

<a name="Group+getGroups"></a>

### group.getGroups() ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
Get the groups within the group

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Array.&lt;Group&gt;](#Group)</code> - An array of child groups  
<a name="Group+getID"></a>

### group.getID() ⇒ <code>string</code>
Get the group ID

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>string</code> - The ID of the group  
<a name="Group+getTitle"></a>

### group.getTitle() ⇒ <code>string</code>
Get the group title

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>string</code> - The title of the group  
<a name="Group+isForeign"></a>

### group.isForeign() ⇒ <code>Boolean</code>
Check if the group is foreign (from another archive)

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Boolean</code> - True if it is foreign  
<a name="Group+isInTrash"></a>

### group.isInTrash() ⇒ <code>Boolean</code>
Check if the group is in the trash

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Boolean</code> - Whether or not the group is within the trash group  
<a name="Group+isShared"></a>

### group.isShared() ⇒ <code>Boolean</code>
Check if the group is shared

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Boolean</code> - True if the group is a shared group  
<a name="Group+isTrash"></a>

### group.isTrash() ⇒ <code>Boolean</code>
Check if the group is used for trash

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Boolean</code> - Whether or not the group is the trash group  
<a name="Group+moveTo"></a>

### group.moveTo(target) ⇒ <code>[Group](#Group)</code>
Move the group to another group or archive

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - Self  

| Param | Type | Description |
| --- | --- | --- |
| target | <code>[Group](#Group)</code> &#124; <code>[Archive](#Archive)</code> | The destination Group or Archive instance |

<a name="Group+moveToGroup"></a>

### ~~group.moveToGroup(group) ⇒ <code>[Group](#Group)</code>~~
***Deprecated***

Move the group into another

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - Returns self  
**See**: moveTo  

| Param | Type | Description |
| --- | --- | --- |
| group | <code>[Group](#Group)</code> | The target group (new parent) |

<a name="Group+setAttribute"></a>

### group.setAttribute(attributeName, value) ⇒ <code>[Group](#Group)</code>
Set an attribute

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - Returns self  

| Param | Type | Description |
| --- | --- | --- |
| attributeName | <code>string</code> | The name of the attribute |
| value | <code>string</code> | The value to set |

<a name="Group+setTitle"></a>

### group.setTitle(title) ⇒ <code>[Group](#Group)</code>
Set the group title

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - Returns self  

| Param | Type | Description |
| --- | --- | --- |
| title | <code>string</code> | The title of the group |

<a name="Group+toObject"></a>

### group.toObject(outputFlags) ⇒ <code>Object</code>
Export group to object

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Object</code> - The group, in raw object form  

| Param | Type | Description |
| --- | --- | --- |
| outputFlags | <code>Number</code> | Bitwise options for outputting entries and child groups |

**Example**  
```js
// output defaults (entries and sub groups)
     group.toObject()
```
**Example**  
```js
// output only entries
     group.toObject(Group.OutputFlag.Entries)
```
**Example**  
```js
// output only the group info
     group.toObject(Group.OutputFlag.OnlyGroup)
```
<a name="Group+toString"></a>

### group.toString(outputFlags) ⇒ <code>string</code>
Export the group to a JSON string

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>string</code> - The group (and entries) in JSON string format  
**See**: toObject  

| Param | Type | Description |
| --- | --- | --- |
| outputFlags | <code>Number</code> | Output configuration flags to pass to `toObject` |

<a name="Group+_getArchive"></a>

### group._getArchive() ⇒ <code>[Archive](#Archive)</code>
Get the archive instance reference

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Archive](#Archive)</code> - The archive instance  
**Access:** protected  
<a name="Group+_getRemoteObject"></a>

### group._getRemoteObject() ⇒ <code>Object</code>
Get the remotely-managed object (group)

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>Object</code> - The object instance for the group  
**Access:** protected  
<a name="Group+_getWestley"></a>

### group._getWestley() ⇒ <code>[Westley](#Westley)</code>
Get the delta managing instance for the archive

**Kind**: instance method of <code>[Group](#Group)</code>  
**Returns**: <code>[Westley](#Westley)</code> - The internal Westley object  
**Access:** protected  
<a name="Group+findEntryByID"></a>

### group.inst.findEntryByID(id) ⇒ <code>null</code> &#124; <code>[Entry](#Entry)</code>
Find an entry by its ID

**Kind**: instance method of <code>[Group](#Group)</code>  
**Mixes**: <code>[inst.findEntryByID](#EntryCollection.inst.findEntryByID)</code>  
**Returns**: <code>null</code> &#124; <code>[Entry](#Entry)</code> - Null if not found, or the Entry instance  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The ID to search for |

<a name="Group.Attributes"></a>

### Group.Attributes : <code>enum</code>
Group attribute names

**Kind**: static enum property of <code>[Group](#Group)</code>  
<a name="Group.OutputFlag"></a>

### Group.OutputFlag : <code>enum</code>
Bitwise output flags for `toObject` and `toString`

**Kind**: static enum property of <code>[Group](#Group)</code>  
**See**

- toObject
- toString

<a name="Group.createNew"></a>

### Group.createNew(archive, [parentID]) ⇒ <code>[Group](#Group)</code>
Create a new Group with a delta-manager and parent group ID

**Kind**: static method of <code>[Group](#Group)</code>  
**Returns**: <code>[Group](#Group)</code> - A new group  
**Throws**:

- <code>Error</code> Throws if the target group doesn't exist
- <code>Error</code> Throws if the target group is the trash group,
     or if the target group is within the trash group


| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive to create the group in |
| [parentID] | <code>string</code> | The parent group ID (default is root) |

<a name="Model"></a>

## Model
**Kind**: global class  

* [Model](#Model)
    * [new Model(data)](#new_Model_new)
    * [.get(key, [defaultValue])](#Model+get) ⇒ <code>\*</code>
    * [.getData()](#Model+getData) ⇒ <code>Object</code>
    * [.set(key, value)](#Model+set) ⇒ <code>[Model](#Model)</code>

<a name="new_Model_new"></a>

### new Model(data)
Data modelling helper


| Param | Type |
| --- | --- |
| data | <code>Object</code> | 

<a name="Model+get"></a>

### model.get(key, [defaultValue]) ⇒ <code>\*</code>
Get a value for a property.
 eg. model.get("some.deep.property", 19);

**Kind**: instance method of <code>[Model](#Model)</code>  
**Access:** public  

| Param | Type | Description |
| --- | --- | --- |
| key | <code>string</code> | The key to get the value for. Splits by period '.' for sub-objects. |
| [defaultValue] | <code>\*</code> | A default value to return if the property is not found |

<a name="Model+getData"></a>

### model.getData() ⇒ <code>Object</code>
Get the wrapped object

**Kind**: instance method of <code>[Model](#Model)</code>  
**Access:** public  
<a name="Model+set"></a>

### model.set(key, value) ⇒ <code>[Model](#Model)</code>
Set a property

**Kind**: instance method of <code>[Model](#Model)</code>  
**Returns**: <code>[Model](#Model)</code> - Returns self  
**Access:** public  

| Param | Type | Description |
| --- | --- | --- |
| key | <code>string</code> | The location (property) at which to set a value (eg. "some.nested.prop") |
| value | <code>string</code> &#124; <code>number</code> &#124; <code>Object</code> &#124; <code>\*</code> | The value to set |

<a name="MyButtercupDatasource"></a>

## MyButtercupDatasource ⇐ <code>[TextDatasource](#TextDatasource)</code>
Datasource for the MyButtercup provider

**Kind**: global class  
**Extends:** <code>[TextDatasource](#TextDatasource)</code>  

* [MyButtercupDatasource](#MyButtercupDatasource) ⇐ <code>[TextDatasource](#TextDatasource)</code>
    * [new MyButtercupDatasource(archiveID, accessToken)](#new_MyButtercupDatasource_new)
    * _instance_
        * [.load(credentials)](#MyButtercupDatasource+load) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
        * [.save(archive, credentials)](#MyButtercupDatasource+save) ⇒ <code>Promise</code>
        * [.toObject()](#MyButtercupDatasource+toObject) ⇒ <code>Object</code>
        * [.setContent(content)](#TextDatasource+setContent) ⇒ <code>[TextDatasource](#TextDatasource)</code>
        * [.toString()](#TextDatasource+toString) ⇒ <code>String</code>
    * _static_
        * [.fromObject(obj)](#MyButtercupDatasource.fromObject) ⇒ <code>[MyButtercupDatasource](#MyButtercupDatasource)</code>
        * [.fromString(str, hostCredentials)](#MyButtercupDatasource.fromString) ⇒ <code>[MyButtercupDatasource](#MyButtercupDatasource)</code>

<a name="new_MyButtercupDatasource_new"></a>

### new MyButtercupDatasource(archiveID, accessToken)
Constructor for the datasource


| Param | Type | Description |
| --- | --- | --- |
| archiveID | <code>Number</code> | The ID of the archive |
| accessToken | <code>String</code> | The OAuth access token |

<a name="MyButtercupDatasource+load"></a>

### myButtercupDatasource.load(credentials) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
Load an archive from the datasource

**Kind**: instance method of <code>[MyButtercupDatasource](#MyButtercupDatasource)</code>  
**Overrides:** <code>[load](#TextDatasource+load)</code>  
**Returns**: <code>[Promise.&lt;Archive&gt;](#Archive)</code> - A promise that resolves with an Archive instance  

| Param | Type | Description |
| --- | --- | --- |
| credentials | <code>[Credentials](#Credentials)</code> | Credentials instance |

<a name="MyButtercupDatasource+save"></a>

### myButtercupDatasource.save(archive, credentials) ⇒ <code>Promise</code>
Save an archive

**Kind**: instance method of <code>[MyButtercupDatasource](#MyButtercupDatasource)</code>  
**Overrides:** <code>[save](#TextDatasource+save)</code>  
**Returns**: <code>Promise</code> - A promise that resolves once saving is complete  

| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive to save |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials to use for saving (master password) |

<a name="MyButtercupDatasource+toObject"></a>

### myButtercupDatasource.toObject() ⇒ <code>Object</code>
Convert the datasource to an object

**Kind**: instance method of <code>[MyButtercupDatasource](#MyButtercupDatasource)</code>  
**Overrides:** <code>[toObject](#TextDatasource+toObject)</code>  
**Returns**: <code>Object</code> - The object representation  
<a name="TextDatasource+setContent"></a>

### myButtercupDatasource.setContent(content) ⇒ <code>[TextDatasource](#TextDatasource)</code>
Set the text content

**Kind**: instance method of <code>[MyButtercupDatasource](#MyButtercupDatasource)</code>  
**Returns**: <code>[TextDatasource](#TextDatasource)</code> - Self  

| Param | Type | Description |
| --- | --- | --- |
| content | <code>String</code> | The encrypted text content |

<a name="TextDatasource+toString"></a>

### myButtercupDatasource.toString() ⇒ <code>String</code>
Output the datasource configuration as a string

**Kind**: instance method of <code>[MyButtercupDatasource](#MyButtercupDatasource)</code>  
**Returns**: <code>String</code> - The string representation of the datasource  
<a name="MyButtercupDatasource.fromObject"></a>

### MyButtercupDatasource.fromObject(obj) ⇒ <code>[MyButtercupDatasource](#MyButtercupDatasource)</code>
Create a datasource instance from an object

**Kind**: static method of <code>[MyButtercupDatasource](#MyButtercupDatasource)</code>  
**Returns**: <code>[MyButtercupDatasource](#MyButtercupDatasource)</code> - A datasource instance  
**Throws**:

- <code>Error</code> Throws if the type is not recognised


| Param | Type | Description |
| --- | --- | --- |
| obj | <code>Object</code> | The object to create an instance from |

<a name="MyButtercupDatasource.fromString"></a>

### MyButtercupDatasource.fromString(str, hostCredentials) ⇒ <code>[MyButtercupDatasource](#MyButtercupDatasource)</code>
Create a datasource from a string

**Kind**: static method of <code>[MyButtercupDatasource](#MyButtercupDatasource)</code>  
**Returns**: <code>[MyButtercupDatasource](#MyButtercupDatasource)</code> - A datasource instance  
**See**: MyButtercupDatasource.fromObject  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>String</code> | The string representation of a datasource |
| hostCredentials | <code>[Credentials](#Credentials)</code> | The credentials for the remote provider |

<a name="NextcloudDatasource"></a>

## NextcloudDatasource ⇐ <code>[OwnCloudDatasource](#OwnCloudDatasource)</code>
Datasource for Nextcloud archives

**Kind**: global class  
**Extends:** <code>[OwnCloudDatasource](#OwnCloudDatasource)</code>  

* [NextcloudDatasource](#NextcloudDatasource) ⇐ <code>[OwnCloudDatasource](#OwnCloudDatasource)</code>
    * [.toObject()](#NextcloudDatasource+toObject) ⇒ <code>Object</code>
    * [.getArchivePath()](#WebDAVDatasource+getArchivePath) ⇒ <code>string</code>
    * [.getRemoteEndpoint()](#WebDAVDatasource+getRemoteEndpoint) ⇒ <code>string</code>
    * [.load(credentials)](#WebDAVDatasource+load) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
    * [.save(archive, credentials)](#WebDAVDatasource+save) ⇒ <code>Promise</code>

<a name="NextcloudDatasource+toObject"></a>

### nextcloudDatasource.toObject() ⇒ <code>Object</code>
Output the datasource as an object

**Kind**: instance method of <code>[NextcloudDatasource](#NextcloudDatasource)</code>  
**Overrides:** <code>[toObject](#OwnCloudDatasource+toObject)</code>  
**Returns**: <code>Object</code> - An object describing the datasource  
<a name="WebDAVDatasource+getArchivePath"></a>

### nextcloudDatasource.getArchivePath() ⇒ <code>string</code>
Get the path of the archive on the server

**Kind**: instance method of <code>[NextcloudDatasource](#NextcloudDatasource)</code>  
**Returns**: <code>string</code> - The path  
<a name="WebDAVDatasource+getRemoteEndpoint"></a>

### nextcloudDatasource.getRemoteEndpoint() ⇒ <code>string</code>
Get the remote endpoint URI (no resource path)

**Kind**: instance method of <code>[NextcloudDatasource](#NextcloudDatasource)</code>  
**Returns**: <code>string</code> - The endpoint  
<a name="WebDAVDatasource+load"></a>

### nextcloudDatasource.load(credentials) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
Load the archive from the datasource

**Kind**: instance method of <code>[NextcloudDatasource](#NextcloudDatasource)</code>  
**Returns**: <code>[Promise.&lt;Archive&gt;](#Archive)</code> - A promise resolving with the archive  

| Param | Type | Description |
| --- | --- | --- |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials for archive decryption |

<a name="WebDAVDatasource+save"></a>

### nextcloudDatasource.save(archive, credentials) ⇒ <code>Promise</code>
Save an archive to the WebDAV service

**Kind**: instance method of <code>[NextcloudDatasource](#NextcloudDatasource)</code>  
**Returns**: <code>Promise</code> - A promise resolving when the save is complete  

| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive to save |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials for encryption |

<a name="OwnCloudDatasource"></a>

## OwnCloudDatasource ⇐ <code>[WebDAVDatasource](#WebDAVDatasource)</code>
Datasource for OwnCloud archives

**Kind**: global class  
**Extends:** <code>[WebDAVDatasource](#WebDAVDatasource)</code>  

* [OwnCloudDatasource](#OwnCloudDatasource) ⇐ <code>[WebDAVDatasource](#WebDAVDatasource)</code>
    * [new OwnCloudDatasource(owncloudURL, resourcePath, credentials)](#new_OwnCloudDatasource_new)
    * [.toObject()](#OwnCloudDatasource+toObject) ⇒ <code>Object</code>
    * [.getArchivePath()](#WebDAVDatasource+getArchivePath) ⇒ <code>string</code>
    * [.getRemoteEndpoint()](#WebDAVDatasource+getRemoteEndpoint) ⇒ <code>string</code>
    * [.load(credentials)](#WebDAVDatasource+load) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
    * [.save(archive, credentials)](#WebDAVDatasource+save) ⇒ <code>Promise</code>

<a name="new_OwnCloudDatasource_new"></a>

### new OwnCloudDatasource(owncloudURL, resourcePath, credentials)
Datasource for Owncloud connections


| Param | Type | Description |
| --- | --- | --- |
| owncloudURL | <code>String</code> | The URL to the owncloud instance, without "remote.php/webdav" etc. |
| resourcePath | <code>String</code> | The file path |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials (username/password) for owncloud |

<a name="OwnCloudDatasource+toObject"></a>

### ownCloudDatasource.toObject() ⇒ <code>Object</code>
Output the datasource as an object

**Kind**: instance method of <code>[OwnCloudDatasource](#OwnCloudDatasource)</code>  
**Overrides:** <code>[toObject](#WebDAVDatasource+toObject)</code>  
**Returns**: <code>Object</code> - An object describing the datasource  
<a name="WebDAVDatasource+getArchivePath"></a>

### ownCloudDatasource.getArchivePath() ⇒ <code>string</code>
Get the path of the archive on the server

**Kind**: instance method of <code>[OwnCloudDatasource](#OwnCloudDatasource)</code>  
**Returns**: <code>string</code> - The path  
<a name="WebDAVDatasource+getRemoteEndpoint"></a>

### ownCloudDatasource.getRemoteEndpoint() ⇒ <code>string</code>
Get the remote endpoint URI (no resource path)

**Kind**: instance method of <code>[OwnCloudDatasource](#OwnCloudDatasource)</code>  
**Returns**: <code>string</code> - The endpoint  
<a name="WebDAVDatasource+load"></a>

### ownCloudDatasource.load(credentials) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
Load the archive from the datasource

**Kind**: instance method of <code>[OwnCloudDatasource](#OwnCloudDatasource)</code>  
**Returns**: <code>[Promise.&lt;Archive&gt;](#Archive)</code> - A promise resolving with the archive  

| Param | Type | Description |
| --- | --- | --- |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials for archive decryption |

<a name="WebDAVDatasource+save"></a>

### ownCloudDatasource.save(archive, credentials) ⇒ <code>Promise</code>
Save an archive to the WebDAV service

**Kind**: instance method of <code>[OwnCloudDatasource](#OwnCloudDatasource)</code>  
**Returns**: <code>Promise</code> - A promise resolving when the save is complete  

| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive to save |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials for encryption |

<a name="TextDatasource"></a>

## TextDatasource
Datasource for text input and output

**Kind**: global class  

* [TextDatasource](#TextDatasource)
    * [new TextDatasource(content)](#new_TextDatasource_new)
    * _instance_
        * [.load(credentials, [emptyCreatesNew])](#TextDatasource+load) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
        * [.save(archive, credentials)](#TextDatasource+save) ⇒ <code>Promise.&lt;string&gt;</code>
        * [.setContent(content)](#TextDatasource+setContent) ⇒ <code>[TextDatasource](#TextDatasource)</code>
        * [.toObject()](#TextDatasource+toObject) ⇒ <code>Object</code>
        * [.toString()](#TextDatasource+toString) ⇒ <code>String</code>
    * _static_
        * ~~[.setDeferredEncodingHandlers(decodeHandler, encodeHandler)](#TextDatasource.setDeferredEncodingHandlers)~~

<a name="new_TextDatasource_new"></a>

### new TextDatasource(content)
Constructor for the text datasource


| Param | Type | Description |
| --- | --- | --- |
| content | <code>string</code> | The content to load from |

<a name="TextDatasource+load"></a>

### textDatasource.load(credentials, [emptyCreatesNew]) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
Load from the stored content using a password to decrypt

**Kind**: instance method of <code>[TextDatasource](#TextDatasource)</code>  
**Returns**: <code>[Promise.&lt;Archive&gt;](#Archive)</code> - A promise that resolves with an open archive  

| Param | Type | Description |
| --- | --- | --- |
| credentials | <code>[Credentials](#Credentials)</code> | The password or Credentials instance to decrypt with |
| [emptyCreatesNew] | <code>Boolean</code> | Create a new Archive instance if text contents are empty (defaults to false) |

<a name="TextDatasource+save"></a>

### textDatasource.save(archive, credentials) ⇒ <code>Promise.&lt;string&gt;</code>
Save an archive with a password

**Kind**: instance method of <code>[TextDatasource](#TextDatasource)</code>  
**Returns**: <code>Promise.&lt;string&gt;</code> - A promise resolving with the encrypted content  

| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive to save |
| credentials | <code>[Credentials](#Credentials)</code> | The Credentials instance to encrypt with |

<a name="TextDatasource+setContent"></a>

### textDatasource.setContent(content) ⇒ <code>[TextDatasource](#TextDatasource)</code>
Set the text content

**Kind**: instance method of <code>[TextDatasource](#TextDatasource)</code>  
**Returns**: <code>[TextDatasource](#TextDatasource)</code> - Self  

| Param | Type | Description |
| --- | --- | --- |
| content | <code>String</code> | The encrypted text content |

<a name="TextDatasource+toObject"></a>

### textDatasource.toObject() ⇒ <code>Object</code>
Output the datasource as an object

**Kind**: instance method of <code>[TextDatasource](#TextDatasource)</code>  
**Returns**: <code>Object</code> - The object representation  
<a name="TextDatasource+toString"></a>

### textDatasource.toString() ⇒ <code>String</code>
Output the datasource configuration as a string

**Kind**: instance method of <code>[TextDatasource](#TextDatasource)</code>  
**Returns**: <code>String</code> - The string representation of the datasource  
<a name="TextDatasource.setDeferredEncodingHandlers"></a>

### ~~TextDatasource.setDeferredEncodingHandlers(decodeHandler, encodeHandler)~~
***Deprecated***

Set the deferred handlers for encryption/decryption of the text-based payload
The load and save procedures can defer their work (packing and encryption) to external callbacks,
essentially enabling custom crypto support. While this is not recommended, it makes it possible
to at least perform the crypto *elsewhere*. This was designed for use on mobile platforms where
crypto support may be limited outside of a webview with SubtleCrypto support.

**Kind**: static method of <code>[TextDatasource](#TextDatasource)</code>  

| Param | Type | Description |
| --- | --- | --- |
| decodeHandler | <code>function</code> &#124; <code>null</code> | The callback function to use for decoding/decryption. Use  `null` to reset it to the built-in. The function expects 2 parameters: The encrypted text and  a credentials instance (that must have a password, 'keyfile' or both). |
| encodeHandler | <code>function</code> &#124; <code>null</code> | The callback function to use for encoding/encryption. Use  `null` to reset it to the built-in. The function expects 2 parameters: The history array and  a credentials instance (that must have a password, 'keyfile' or both). |

<a name="WebDAVDatasource"></a>

## WebDAVDatasource ⇐ <code>[TextDatasource](#TextDatasource)</code>
**Kind**: global class  
**Extends:** <code>[TextDatasource](#TextDatasource)</code>  

* [WebDAVDatasource](#WebDAVDatasource) ⇐ <code>[TextDatasource](#TextDatasource)</code>
    * [new WebDAVDatasource()](#new_WebDAVDatasource_new)
    * [new WebDAVDatasource(endpoint, webDAVPath, [credentials])](#new_WebDAVDatasource_new)
    * [.getArchivePath()](#WebDAVDatasource+getArchivePath) ⇒ <code>string</code>
    * [.getRemoteEndpoint()](#WebDAVDatasource+getRemoteEndpoint) ⇒ <code>string</code>
    * [.load(credentials)](#WebDAVDatasource+load) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
    * [.save(archive, credentials)](#WebDAVDatasource+save) ⇒ <code>Promise</code>
    * [.toObject()](#WebDAVDatasource+toObject) ⇒ <code>Object</code>
    * [.setContent(content)](#TextDatasource+setContent) ⇒ <code>[TextDatasource](#TextDatasource)</code>
    * [.toString()](#TextDatasource+toString) ⇒ <code>String</code>

<a name="new_WebDAVDatasource_new"></a>

### new WebDAVDatasource()
WebDAV datasource for reading and writing remote archives

<a name="new_WebDAVDatasource_new"></a>

### new WebDAVDatasource(endpoint, webDAVPath, [credentials])
Constructor for the datasource


| Param | Type | Description |
| --- | --- | --- |
| endpoint | <code>string</code> | URL for the WebDAV service (without resource path) |
| webDAVPath | <code>string</code> | Resource path on the WebDAV service |
| [credentials] | <code>[Credentials](#Credentials)</code> | Credentials (username/password) for the WebDAV service |

<a name="WebDAVDatasource+getArchivePath"></a>

### webDAVDatasource.getArchivePath() ⇒ <code>string</code>
Get the path of the archive on the server

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Returns**: <code>string</code> - The path  
<a name="WebDAVDatasource+getRemoteEndpoint"></a>

### webDAVDatasource.getRemoteEndpoint() ⇒ <code>string</code>
Get the remote endpoint URI (no resource path)

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Returns**: <code>string</code> - The endpoint  
<a name="WebDAVDatasource+load"></a>

### webDAVDatasource.load(credentials) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
Load the archive from the datasource

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Overrides:** <code>[load](#TextDatasource+load)</code>  
**Returns**: <code>[Promise.&lt;Archive&gt;](#Archive)</code> - A promise resolving with the archive  

| Param | Type | Description |
| --- | --- | --- |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials for archive decryption |

<a name="WebDAVDatasource+save"></a>

### webDAVDatasource.save(archive, credentials) ⇒ <code>Promise</code>
Save an archive to the WebDAV service

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Overrides:** <code>[save](#TextDatasource+save)</code>  
**Returns**: <code>Promise</code> - A promise resolving when the save is complete  

| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive to save |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials for encryption |

<a name="WebDAVDatasource+toObject"></a>

### webDAVDatasource.toObject() ⇒ <code>Object</code>
Output the datasource as an object

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Overrides:** <code>[toObject](#TextDatasource+toObject)</code>  
**Returns**: <code>Object</code> - An object describing the datasource  
<a name="TextDatasource+setContent"></a>

### webDAVDatasource.setContent(content) ⇒ <code>[TextDatasource](#TextDatasource)</code>
Set the text content

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Returns**: <code>[TextDatasource](#TextDatasource)</code> - Self  

| Param | Type | Description |
| --- | --- | --- |
| content | <code>String</code> | The encrypted text content |

<a name="TextDatasource+toString"></a>

### webDAVDatasource.toString() ⇒ <code>String</code>
Output the datasource configuration as a string

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Returns**: <code>String</code> - The string representation of the datasource  
<a name="WebDAVDatasource"></a>

## WebDAVDatasource
**Kind**: global class  

* [WebDAVDatasource](#WebDAVDatasource)
    * [new WebDAVDatasource()](#new_WebDAVDatasource_new)
    * [new WebDAVDatasource(endpoint, webDAVPath, [credentials])](#new_WebDAVDatasource_new)
    * [.getArchivePath()](#WebDAVDatasource+getArchivePath) ⇒ <code>string</code>
    * [.getRemoteEndpoint()](#WebDAVDatasource+getRemoteEndpoint) ⇒ <code>string</code>
    * [.load(credentials)](#WebDAVDatasource+load) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
    * [.save(archive, credentials)](#WebDAVDatasource+save) ⇒ <code>Promise</code>
    * [.toObject()](#WebDAVDatasource+toObject) ⇒ <code>Object</code>
    * [.setContent(content)](#TextDatasource+setContent) ⇒ <code>[TextDatasource](#TextDatasource)</code>
    * [.toString()](#TextDatasource+toString) ⇒ <code>String</code>

<a name="new_WebDAVDatasource_new"></a>

### new WebDAVDatasource()
WebDAV datasource for reading and writing remote archives

<a name="new_WebDAVDatasource_new"></a>

### new WebDAVDatasource(endpoint, webDAVPath, [credentials])
Constructor for the datasource


| Param | Type | Description |
| --- | --- | --- |
| endpoint | <code>string</code> | URL for the WebDAV service (without resource path) |
| webDAVPath | <code>string</code> | Resource path on the WebDAV service |
| [credentials] | <code>[Credentials](#Credentials)</code> | Credentials (username/password) for the WebDAV service |

<a name="WebDAVDatasource+getArchivePath"></a>

### webDAVDatasource.getArchivePath() ⇒ <code>string</code>
Get the path of the archive on the server

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Returns**: <code>string</code> - The path  
<a name="WebDAVDatasource+getRemoteEndpoint"></a>

### webDAVDatasource.getRemoteEndpoint() ⇒ <code>string</code>
Get the remote endpoint URI (no resource path)

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Returns**: <code>string</code> - The endpoint  
<a name="WebDAVDatasource+load"></a>

### webDAVDatasource.load(credentials) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
Load the archive from the datasource

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Overrides:** <code>[load](#TextDatasource+load)</code>  
**Returns**: <code>[Promise.&lt;Archive&gt;](#Archive)</code> - A promise resolving with the archive  

| Param | Type | Description |
| --- | --- | --- |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials for archive decryption |

<a name="WebDAVDatasource+save"></a>

### webDAVDatasource.save(archive, credentials) ⇒ <code>Promise</code>
Save an archive to the WebDAV service

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Overrides:** <code>[save](#TextDatasource+save)</code>  
**Returns**: <code>Promise</code> - A promise resolving when the save is complete  

| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive to save |
| credentials | <code>[Credentials](#Credentials)</code> | The credentials for encryption |

<a name="WebDAVDatasource+toObject"></a>

### webDAVDatasource.toObject() ⇒ <code>Object</code>
Output the datasource as an object

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Overrides:** <code>[toObject](#TextDatasource+toObject)</code>  
**Returns**: <code>Object</code> - An object describing the datasource  
<a name="TextDatasource+setContent"></a>

### webDAVDatasource.setContent(content) ⇒ <code>[TextDatasource](#TextDatasource)</code>
Set the text content

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Returns**: <code>[TextDatasource](#TextDatasource)</code> - Self  

| Param | Type | Description |
| --- | --- | --- |
| content | <code>String</code> | The encrypted text content |

<a name="TextDatasource+toString"></a>

### webDAVDatasource.toString() ⇒ <code>String</code>
Output the datasource configuration as a string

**Kind**: instance method of <code>[WebDAVDatasource](#WebDAVDatasource)</code>  
**Returns**: <code>String</code> - The string representation of the datasource  
<a name="Westley"></a>

## Westley
**Kind**: global class  

* [Westley](#Westley)
    * [new Westley()](#new_Westley_new)
    * [.readOnly](#Westley+readOnly)
    * [.readOnly](#Westley+readOnly)
    * [.clear()](#Westley+clear) ⇒ <code>[Westley](#Westley)</code>
    * [.execute(command, [append])](#Westley+execute) ⇒ <code>[Westley](#Westley)</code>
    * [.getDataset()](#Westley+getDataset) ⇒ <code>Object</code>
    * [.getHistory()](#Westley+getHistory) ⇒ <code>Array.&lt;String&gt;</code>
    * [.pad()](#Westley+pad) ⇒ <code>[Westley](#Westley)</code>
    * [._getCommandForKey(commandKey)](#Westley+_getCommandForKey) ⇒ <code>Command</code>

<a name="new_Westley_new"></a>

### new Westley()
Westley. Archive object dataset and history manager. Handles parsing and
revenge for the princess.

<a name="Westley+readOnly"></a>

### westley.readOnly
**Kind**: instance property of <code>[Westley](#Westley)</code>  
**Access:** public  
**Properties**

| Name | Type |
| --- | --- |
| readOnly | <code>Boolean</code> | 

<a name="Westley+readOnly"></a>

### westley.readOnly
Set the read only value

**Kind**: instance property of <code>[Westley](#Westley)</code>  

| Param | Type | Description |
| --- | --- | --- |
| newRO | <code>Boolean</code> | The new value |

<a name="Westley+clear"></a>

### westley.clear() ⇒ <code>[Westley](#Westley)</code>
Clear the dataset and history

**Kind**: instance method of <code>[Westley](#Westley)</code>  
**Returns**: <code>[Westley](#Westley)</code> - Returns self  
<a name="Westley+execute"></a>

### westley.execute(command, [append]) ⇒ <code>[Westley](#Westley)</code>
Execute a command - stored in history and modifies the dataset

**Kind**: instance method of <code>[Westley](#Westley)</code>  
**Returns**: <code>[Westley](#Westley)</code> - Returns self  

| Param | Type | Description |
| --- | --- | --- |
| command | <code>String</code> | The command to execute |
| [append] | <code>Boolean</code> | Wether to append to the end of the history list (default true) |

<a name="Westley+getDataset"></a>

### westley.getDataset() ⇒ <code>Object</code>
Get the core dataset

**Kind**: instance method of <code>[Westley](#Westley)</code>  
**Returns**: <code>Object</code> - The dataset object  
<a name="Westley+getHistory"></a>

### westley.getHistory() ⇒ <code>Array.&lt;String&gt;</code>
Get the history (deltas)

**Kind**: instance method of <code>[Westley](#Westley)</code>  
**Returns**: <code>Array.&lt;String&gt;</code> - The command array (history)  
<a name="Westley+pad"></a>

### westley.pad() ⇒ <code>[Westley](#Westley)</code>
Insert a padding in the archive (used for delta tracking)

**Kind**: instance method of <code>[Westley](#Westley)</code>  
**Returns**: <code>[Westley](#Westley)</code> - Returns self  
<a name="Westley+_getCommandForKey"></a>

### westley._getCommandForKey(commandKey) ⇒ <code>Command</code>
Gets a command by its key from the cache with its dependencies injected

**Kind**: instance method of <code>[Westley](#Westley)</code>  
**Returns**: <code>Command</code> - Returns the command  
**Access:** protected  

| Param | Type | Description |
| --- | --- | --- |
| commandKey | <code>String</code> | The key of the command |

<a name="Workspace"></a>

## Workspace
**Kind**: global class  

* [Workspace](#Workspace)
    * [new Workspace()](#new_Workspace_new)
    * [.primary](#Workspace+primary) : <code>[WorkspaceItem](#WorkspaceItem)</code>
    * [.addSharedArchive(archive, datasource, masterCredentials, [saveable])](#Workspace+addSharedArchive) ⇒ <code>[Workspace](#Workspace)</code>
    * [.getAllItems()](#Workspace+getAllItems) ⇒ <code>[Array.&lt;WorkspaceItem&gt;](#WorkspaceItem)</code>
    * [.getSaveableItems()](#Workspace+getSaveableItems) ⇒ <code>[Array.&lt;WorkspaceItem&gt;](#WorkspaceItem)</code>
    * [.imbue()](#Workspace+imbue) ⇒ <code>[Workspace](#Workspace)</code>
    * [.localDiffersFromRemote()](#Workspace+localDiffersFromRemote) ⇒ <code>Promise.&lt;Boolean&gt;</code>
    * [.mergeItemFromRemote(item)](#Workspace+mergeItemFromRemote) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
    * [.mergeSaveablesFromRemote()](#Workspace+mergeSaveablesFromRemote) ⇒ <code>Promise.&lt;Array.&lt;Archive&gt;&gt;</code>
    * [.save()](#Workspace+save) ⇒ <code>Promise</code>
    * [.setPrimaryArchive(archive, datasource, masterCredentials)](#Workspace+setPrimaryArchive) ⇒ <code>[Workspace](#Workspace)</code>

<a name="new_Workspace_new"></a>

### new Workspace()
Workspace

<a name="Workspace+primary"></a>

### workspace.primary : <code>[WorkspaceItem](#WorkspaceItem)</code>
The primary archive item

**Kind**: instance property of <code>[Workspace](#Workspace)</code>  
**Access:** public  
<a name="Workspace+addSharedArchive"></a>

### workspace.addSharedArchive(archive, datasource, masterCredentials, [saveable]) ⇒ <code>[Workspace](#Workspace)</code>
Add a shared archive item

**Kind**: instance method of <code>[Workspace](#Workspace)</code>  
**Returns**: <code>[Workspace](#Workspace)</code> - Self  

| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The archive instance |
| datasource | <code>[TextDatasource](#TextDatasource)</code> | The datasource instance |
| masterCredentials | <code>[Credentials](#Credentials)</code> | The master credentials (password) |
| [saveable] | <code>Boolean</code> | Whether the archive is remotely saveable or not (default: true) |

<a name="Workspace+getAllItems"></a>

### workspace.getAllItems() ⇒ <code>[Array.&lt;WorkspaceItem&gt;](#WorkspaceItem)</code>
Get all archive items

**Kind**: instance method of <code>[Workspace](#Workspace)</code>  
**Returns**: <code>[Array.&lt;WorkspaceItem&gt;](#WorkspaceItem)</code> - All of the items  
<a name="Workspace+getSaveableItems"></a>

### workspace.getSaveableItems() ⇒ <code>[Array.&lt;WorkspaceItem&gt;](#WorkspaceItem)</code>
Get all the saveable items

**Kind**: instance method of <code>[Workspace](#Workspace)</code>  
**Returns**: <code>[Array.&lt;WorkspaceItem&gt;](#WorkspaceItem)</code> - All of the saveable items  
<a name="Workspace+imbue"></a>

### workspace.imbue() ⇒ <code>[Workspace](#Workspace)</code>
Imbue the primary archive with shared groups from all of the other archives

**Kind**: instance method of <code>[Workspace](#Workspace)</code>  
**Returns**: <code>[Workspace](#Workspace)</code> - Self  
**Throws**:

- <code>Error</code> Throws if the primary archive is not set

<a name="Workspace+localDiffersFromRemote"></a>

### workspace.localDiffersFromRemote() ⇒ <code>Promise.&lt;Boolean&gt;</code>
Detect whether the local archives (in memory) differ from their remote copies
Fetches the remote copies from their datasources and detects differences between
them and their local counterparts. Does not change/update the local items.

**Kind**: instance method of <code>[Workspace](#Workspace)</code>  
**Returns**: <code>Promise.&lt;Boolean&gt;</code> - A promise that resolves with a boolean - true if
     there are differences, false if there is not  
<a name="Workspace+mergeItemFromRemote"></a>

### workspace.mergeItemFromRemote(item) ⇒ <code>[Promise.&lt;Archive&gt;](#Archive)</code>
Merge an item from its remote counterpart
Detects differences between a local and a remote item, and merges the
two copies together.

**Kind**: instance method of <code>[Workspace](#Workspace)</code>  
**Returns**: <code>[Promise.&lt;Archive&gt;](#Archive)</code> - A promise that resolves with the newly merged archive -
     This archive is automatically saved over the original local copy.  

| Param | Type | Description |
| --- | --- | --- |
| item | <code>[WorkspaceItem](#WorkspaceItem)</code> | The local item |

<a name="Workspace+mergeSaveablesFromRemote"></a>

### workspace.mergeSaveablesFromRemote() ⇒ <code>Promise.&lt;Array.&lt;Archive&gt;&gt;</code>
Merge all saveable remote copies into their local counterparts

**Kind**: instance method of <code>[Workspace](#Workspace)</code>  
**Returns**: <code>Promise.&lt;Array.&lt;Archive&gt;&gt;</code> - A promise that resolves with an array of merged Archives  
**See**

- mergeItemFromRemote
- embue

<a name="Workspace+save"></a>

### workspace.save() ⇒ <code>Promise</code>
Save all saveable archives to their remotes

**Kind**: instance method of <code>[Workspace](#Workspace)</code>  
**Returns**: <code>Promise</code> - A promise that resolves when all saveable archives have been saved  
<a name="Workspace+setPrimaryArchive"></a>

### workspace.setPrimaryArchive(archive, datasource, masterCredentials) ⇒ <code>[Workspace](#Workspace)</code>
Set the primary archive

**Kind**: instance method of <code>[Workspace](#Workspace)</code>  
**Returns**: <code>[Workspace](#Workspace)</code> - Self  

| Param | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | The Archive instance |
| datasource | <code>[TextDatasource](#TextDatasource)</code> | The datasource instance |
| masterCredentials | <code>[Credentials](#Credentials)</code> | The master password |

<a name="LocalStorageInterface"></a>

## LocalStorageInterface ⇐ <code>StorageInterface</code>
Interface for localStorage

**Kind**: global class  
**Extends:** <code>StorageInterface</code>  

* [LocalStorageInterface](#LocalStorageInterface) ⇐ <code>StorageInterface</code>
    * [.getAllKeys()](#LocalStorageInterface+getAllKeys) ⇒ <code>Promise.&lt;Array.&lt;String&gt;&gt;</code>
    * [.getValue(name)](#LocalStorageInterface+getValue) ⇒ <code>Promise.&lt;String&gt;</code>
    * [.setValue(name, value)](#LocalStorageInterface+setValue) ⇒ <code>Promise</code>

<a name="LocalStorageInterface+getAllKeys"></a>

### localStorageInterface.getAllKeys() ⇒ <code>Promise.&lt;Array.&lt;String&gt;&gt;</code>
Get all keys from storage

**Kind**: instance method of <code>[LocalStorageInterface](#LocalStorageInterface)</code>  
**Returns**: <code>Promise.&lt;Array.&lt;String&gt;&gt;</code> - A promise that resolves with an array of keys  
<a name="LocalStorageInterface+getValue"></a>

### localStorageInterface.getValue(name) ⇒ <code>Promise.&lt;String&gt;</code>
Get the value of a key

**Kind**: instance method of <code>[LocalStorageInterface](#LocalStorageInterface)</code>  
**Returns**: <code>Promise.&lt;String&gt;</code> - A promise that resolves with the value  

| Param | Type | Description |
| --- | --- | --- |
| name | <code>String</code> | The key name |

<a name="LocalStorageInterface+setValue"></a>

### localStorageInterface.setValue(name, value) ⇒ <code>Promise</code>
Set the value for a key

**Kind**: instance method of <code>[LocalStorageInterface](#LocalStorageInterface)</code>  
**Returns**: <code>Promise</code> - A promise that resolves when the value is set  

| Param | Type | Description |
| --- | --- | --- |
| name | <code>String</code> | The key name |
| value | <code>String</code> | The value to set |

<a name="EntryCollection"></a>

## EntryCollection : <code>Object</code>
**Kind**: global mixin  

* [EntryCollection](#EntryCollection) : <code>Object</code>
    * [.findEntriesByMeta](#EntryCollection.findEntriesByMeta) ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
    * [.findEntriesByProperty](#EntryCollection.findEntriesByProperty) ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
    * [.inst.findEntryByID(id)](#EntryCollection.inst.findEntryByID) ⇒ <code>null</code> &#124; <code>[Entry](#Entry)</code>

<a name="EntryCollection.findEntriesByMeta"></a>

### EntryCollection.findEntriesByMeta ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
Find entries that match a certain meta property

**Kind**: static property of <code>[EntryCollection](#EntryCollection)</code>  
**Returns**: <code>[Array.&lt;Entry&gt;](#Entry)</code> - An array of found entries  

| Param | Type | Description |
| --- | --- | --- |
| metaName | <code>String</code> | The meta property to search for |
| value | <code>RegExp</code> &#124; <code>string</code> | The value to search for |

<a name="EntryCollection.findEntriesByProperty"></a>

### EntryCollection.findEntriesByProperty ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
Find all entries that match a certain property

**Kind**: static property of <code>[EntryCollection](#EntryCollection)</code>  
**Returns**: <code>[Array.&lt;Entry&gt;](#Entry)</code> - An array of found extries  

| Param | Type | Description |
| --- | --- | --- |
| property | <code>string</code> | The property to search with |
| value | <code>RegExp</code> &#124; <code>string</code> | The value to search for |

<a name="EntryCollection.inst.findEntryByID"></a>

### EntryCollection.inst.findEntryByID(id) ⇒ <code>null</code> &#124; <code>[Entry](#Entry)</code>
Find an entry by its ID

**Kind**: static method of <code>[EntryCollection](#EntryCollection)</code>  
**Returns**: <code>null</code> &#124; <code>[Entry](#Entry)</code> - Null if not found, or the Entry instance  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The ID to search for |

<a name="GroupCollection"></a>

## GroupCollection : <code>Object</code>
**Kind**: global mixin  

* [GroupCollection](#GroupCollection) : <code>Object</code>
    * [.findGroupByID](#GroupCollection.findGroupByID) ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
    * [.findGroupsByTitle](#GroupCollection.findGroupsByTitle) ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>

<a name="GroupCollection.findGroupByID"></a>

### GroupCollection.findGroupByID ⇒ <code>[Group](#Group)</code> &#124; <code>null</code>
Find a group by its ID

**Kind**: static property of <code>[GroupCollection](#GroupCollection)</code>  
**Returns**: <code>[Group](#Group)</code> &#124; <code>null</code> - The group or null if not found  

| Param | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | The group ID to search for |

<a name="GroupCollection.findGroupsByTitle"></a>

### GroupCollection.findGroupsByTitle ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
Find groups by their title

**Kind**: static property of <code>[GroupCollection](#GroupCollection)</code>  
**Returns**: <code>[Array.&lt;Group&gt;](#Group)</code> - An array of groups  

| Param | Type | Description |
| --- | --- | --- |
| title | <code>String</code> &#124; <code>RegExp</code> | The group title |

<a name="flattenEntries"></a>

## flattenEntries(archives) ⇒ <code>[Array.&lt;EntrySearchInfo&gt;](#EntrySearchInfo)</code>
Flatten entries into a searchable structure

**Kind**: global function  
**Returns**: <code>[Array.&lt;EntrySearchInfo&gt;](#EntrySearchInfo)</code> - An array of searchable objects  

| Param | Type | Description |
| --- | --- | --- |
| archives | <code>[Array.&lt;Archive&gt;](#Archive)</code> | An array of archives |

<a name="convertEncryptedContentToHistory"></a>

## convertEncryptedContentToHistory(encText, credentials) ⇒ <code>Promise.&lt;Array&gt;</code>
Convert encrypted text to an array of commands (history)

**Kind**: global function  
**Returns**: <code>Promise.&lt;Array&gt;</code> - A promise that resolves with an array of commands  

| Param | Type | Description |
| --- | --- | --- |
| encText | <code>String</code> | The encrypted archive content |
| credentials | <code>[Credentials](#Credentials)</code> | A credentials instance that has a password, keyfile  or both |

<a name="convertHistoryToEncryptedContent"></a>

## convertHistoryToEncryptedContent(historyArr, credentials) ⇒ <code>String</code>
Convert an array of commands (history) to an encrypted string

**Kind**: global function  
**Returns**: <code>String</code> - Encrypted archive contents  

| Param | Type | Description |
| --- | --- | --- |
| historyArr | <code>Array.&lt;String&gt;</code> | An array of commands |
| credentials | <code>[Credentials](#Credentials)</code> | A credentials instance that has a password, keyfile  or both |

<a name="createCredentials"></a>

## createCredentials([type], [data]) ⇒ <code>[Credentials](#Credentials)</code>
Create a credentials adapter
Both `type` and `data` parameters are optional.

**Kind**: global function  
**Returns**: <code>[Credentials](#Credentials)</code> - A credentials adapter  

| Param | Type | Description |
| --- | --- | --- |
| [type] | <code>String</code> | The type of credentials object |
| [data] | <code>Object</code> | The credentials data |


* [createCredentials([type], [data])](#createCredentials) ⇒ <code>[Credentials](#Credentials)</code>
    * [.fromInsecureString(content)](#createCredentials.fromInsecureString) ⇒ <code>[Credentials](#Credentials)</code>
    * [.fromPassword(password)](#createCredentials.fromPassword) ⇒ <code>[Credentials](#Credentials)</code>
    * [.fromSecureString(content, password)](#createCredentials.fromSecureString) ⇒ <code>[Promise.&lt;Credentials&gt;](#Credentials)</code>

<a name="createCredentials.fromInsecureString"></a>

### createCredentials.fromInsecureString(content) ⇒ <code>[Credentials](#Credentials)</code>
Create a credentials instance from an insecure string

**Kind**: static method of <code>[createCredentials](#createCredentials)</code>  
**Returns**: <code>[Credentials](#Credentials)</code> - The credentials instance  

| Param | Type | Description |
| --- | --- | --- |
| content | <code>String</code> | The string format of a credentials instance (insecure) |

<a name="createCredentials.fromPassword"></a>

### createCredentials.fromPassword(password) ⇒ <code>[Credentials](#Credentials)</code>
Create a new credentials instance from a password

**Kind**: static method of <code>[createCredentials](#createCredentials)</code>  
**Returns**: <code>[Credentials](#Credentials)</code> - The credentials instance  

| Param | Type | Description |
| --- | --- | --- |
| password | <code>String</code> | The password to use |

<a name="createCredentials.fromSecureString"></a>

### createCredentials.fromSecureString(content, password) ⇒ <code>[Promise.&lt;Credentials&gt;](#Credentials)</code>
Create a new credentials instance from an encrypted string

**Kind**: static method of <code>[createCredentials](#createCredentials)</code>  
**Returns**: <code>[Promise.&lt;Credentials&gt;](#Credentials)</code> - A promise that resolves with a credentials instance  

| Param | Type | Description |
| --- | --- | --- |
| content | <code>String</code> | The encrypted form of a credentials store |
| password | <code>String</code> | The password to use to decrypt the content |

<a name="addMetaFieldsNonDestructive"></a>

## addMetaFieldsNonDestructive(entry, fields) ⇒ <code>[Array.&lt;EntryFacadeField&gt;](#EntryFacadeField)</code>
Add meta fields to a fields array that are not mentioned in a preset
Facades are creaded by presets which don't mention all meta values (custom user
added items). This method adds the unmentioned items to the facade fields so that
they can be edited as well.

**Kind**: global function  
**Returns**: <code>[Array.&lt;EntryFacadeField&gt;](#EntryFacadeField)</code> - A new array with all combined fields  

| Param | Type | Description |
| --- | --- | --- |
| entry | <code>[Entry](#Entry)</code> | An Entry instance |
| fields | <code>[Array.&lt;EntryFacadeField&gt;](#EntryFacadeField)</code> | An array of fields |

<a name="applyFieldDescriptor"></a>

## applyFieldDescriptor(entry, descriptor)
Apply a facade field descriptor to an entry
Takes data from the descriptor and writes it to the entry.

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| entry | <code>[Entry](#Entry)</code> | The entry to apply to |
| descriptor | <code>[EntryFacadeField](#EntryFacadeField)</code> | The descriptor object |

<a name="consumeEntryFacade"></a>

## consumeEntryFacade(entry, facade)
Process a modified entry facade

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| entry | <code>[Entry](#Entry)</code> | The entry to apply processed data on |
| facade | <code>[EntryFacade](#EntryFacade)</code> | The facade object |

<a name="createEntryFacade"></a>

## createEntryFacade(entry) ⇒ <code>[EntryFacade](#EntryFacade)</code>
Create a data/input facade for an Entry instance

**Kind**: global function  
**Returns**: <code>[EntryFacade](#EntryFacade)</code> - A newly created facade  

| Param | Type | Description |
| --- | --- | --- |
| entry | <code>[Entry](#Entry)</code> | The Entry instance |

<a name="getEntryFacadeType"></a>

## getEntryFacadeType(entry) ⇒ <code>String</code>
Get the facade type for an entry

**Kind**: global function  
**Returns**: <code>String</code> - The facade type  

| Param | Type | Description |
| --- | --- | --- |
| entry | <code>[Entry](#Entry)</code> | The entry instance |

<a name="setEntryValue"></a>

## setEntryValue(entry, property, name, value)
Set a value on an entry

**Kind**: global function  
**Throws**:

- <code>Error</code> Throws if the property type is not recognised


| Param | Type | Description |
| --- | --- | --- |
| entry | <code>[Entry](#Entry)</code> | The entry instance |
| property | <code>String</code> | Type of property ("property"/"meta"/"attribute") |
| name | <code>String</code> | The property name |
| value | <code>String</code> | The value to set |

<a name="dedupe"></a>

## dedupe(arr) ⇒ <code>Array</code>
De-dupe an array

**Kind**: global function  
**Returns**: <code>Array</code> - The de-duped array  

| Param | Type | Description |
| --- | --- | --- |
| arr | <code>Array</code> | The array |

<a name="createFieldDescriptor"></a>

## createFieldDescriptor(entry, title, entryPropertyType, entryPropertyName, options) ⇒ <code>[EntryFacadeField](#EntryFacadeField)</code>
Create a descriptor for a field to be used within a facade

**Kind**: global function  
**Returns**: <code>[EntryFacadeField](#EntryFacadeField)</code> - The field descriptor  

| Param | Type | Description |
| --- | --- | --- |
| entry | <code>[Entry](#Entry)</code> | The entry instance to process |
| title | <code>String</code> | The field title |
| entryPropertyType | <code>String</code> | The type of entry property (property/meta/attribute) |
| entryPropertyName | <code>String</code> | The name of the property |
| options | <code>Object</code> | The options for the field |

<a name="getEntryValue"></a>

## getEntryValue(entry, property, name) ⇒ <code>String</code>
Get a value on an entry for a specific property type

**Kind**: global function  
**Returns**: <code>String</code> - The property value  
**Throws**:

- <code>Error</code> Throws for unknown property types


| Param | Type | Description |
| --- | --- | --- |
| entry | <code>[Entry](#Entry)</code> | The entry instance |
| property | <code>String</code> | The type of entry property (property/meta/attribute) |
| name | <code>String</code> | The property name |

<a name="getValidProperties"></a>

## getValidProperties() ⇒ <code>Array.&lt;String&gt;</code>
Get an array of valid property names

**Kind**: global function  
**Returns**: <code>Array.&lt;String&gt;</code> - An array of names  
<a name="isValidProperty"></a>

## isValidProperty(name) ⇒ <code>Boolean</code>
Check if a property name is valid

**Kind**: global function  
**Returns**: <code>Boolean</code> - True if the name is valid  

| Param | Type | Description |
| --- | --- | --- |
| name | <code>String</code> | The name to check |

<a name="generateUUID"></a>

## generateUUID() ⇒ <code>String</code>
Generate a UUID (v4)

**Kind**: global function  
**Returns**: <code>String</code> - The new UUID  
<a name="findEntriesByCheck"></a>

## findEntriesByCheck(groups, compareFn) ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
Find entry instances by filtering with a compare function

**Kind**: global function  
**Returns**: <code>[Array.&lt;Entry&gt;](#Entry)</code> - An array of found entries  

| Param | Type | Description |
| --- | --- | --- |
| groups | <code>[Array.&lt;Group&gt;](#Group)</code> | The groups to check in |
| compareFn | <code>function</code> | The callback comparison function, return true to keep and false  to strip |

<a name="findGroupsByCheck"></a>

## findGroupsByCheck(groups, compareFn) ⇒ <code>[Array.&lt;Group&gt;](#Group)</code>
Find group instances within groups that satisfy some check

**Kind**: global function  
**Returns**: <code>[Array.&lt;Group&gt;](#Group)</code> - An array of found groups  

| Param | Type | Description |
| --- | --- | --- |
| groups | <code>[Array.&lt;Group&gt;](#Group)</code> | The groups to check within |
| compareFn | <code>function</code> | A comparision function - return true to keep, false to strip |

<a name="getAllEntries"></a>

## getAllEntries(groups) ⇒ <code>[Array.&lt;Entry&gt;](#Entry)</code>
Get all entries within a collection of groups

**Kind**: global function  
**Returns**: <code>[Array.&lt;Entry&gt;](#Entry)</code> - An array of entries  

| Param | Type | Description |
| --- | --- | --- |
| groups | <code>[Array.&lt;Group&gt;](#Group)</code> | An array of groups |

<a name="deriveKeyFromPassword"></a>

## deriveKeyFromPassword(password, salt, rounds, bits) ⇒ <code>Promise.&lt;ArrayBuffer&gt;</code>
Derive a key from a password

**Kind**: global function  
**Returns**: <code>Promise.&lt;ArrayBuffer&gt;</code> - A promise that resolves with an ArrayBuffer  
**See**: checkBrowserSupport  

| Param | Type | Description |
| --- | --- | --- |
| password | <code>String</code> | The password |
| salt | <code>String</code> | The salt |
| rounds | <code>Number</code> | The number of derivation rounds |
| bits | <code>Number</code> | The number of bits for the key |

<a name="patchCorePBKDF"></a>

## patchCorePBKDF(handler)
Perform patching of the PBKDF2 function in iocane

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| handler | <code>function</code> &#124; <code>undefined</code> | Optionally override the internal PBKDF2 engine |

<a name="ArchiveManagerSourceStatus"></a>

## ArchiveManagerSourceStatus : <code>String</code>
Status of a source: locked/unlocked/pending

**Kind**: global typedef  
<a name="UnlockedArchiveManagerSource"></a>

## UnlockedArchiveManagerSource : <code>Object</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| name | <code>String</code> | The name of the source |
| id | <code>String</code> | The ID of the source (UUID) |
| status | <code>[ArchiveManagerSourceStatus](#ArchiveManagerSourceStatus)</code> | The current status of the source |
| type | <code>String</code> | The type of source (eg. dropbox/mybuttercup etc.) |
| workspace | <code>[Workspace](#Workspace)</code> | The archive's workspace |
| sourceCredentials | <code>[Credentials](#Credentials)</code> | Credentials for the remote datasource |
| archiveCredentials | <code>[Credentials](#Credentials)</code> | Credentials for unlocking the archive |

<a name="LockedArchiveManagerSource"></a>

## LockedArchiveManagerSource : <code>Object</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| name | <code>String</code> | The name of the source |
| id | <code>String</code> | The ID of the source (UUID) |
| status | <code>[ArchiveManagerSourceStatus](#ArchiveManagerSourceStatus)</code> | The current status of the source |
| type | <code>String</code> | The type of source (eg. dropbox/mybuttercup etc.) |
| sourceCredentials | <code>String</code> | Encrypted credentials for the remote datasource |
| archiveCredentials | <code>String</code> | Encrypted credentials for unlocking the archive |

<a name="EntrySearchInfo"></a>

## EntrySearchInfo : <code>Object</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| entry | <code>[Entry](#Entry)</code> | The entry |
| archive | <code>[Archive](#Archive)</code> | The associated archive |

<a name="WorkspaceItem"></a>

## WorkspaceItem : <code>Object</code>
Shared workspace item

**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| archive | <code>[Archive](#Archive)</code> | An archive instance |
| password | <code>String</code> | The master password |
| datasource | <code>[TextDatasource](#TextDatasource)</code> | A datasource instance |

<a name="Credentials"></a>

## Credentials : <code>Object</code>
Credentials wrapper

**Kind**: global typedef  

* [Credentials](#Credentials) : <code>Object</code>
    * [.password](#Credentials+password) : <code>String</code> &#124; <code>undefined</code>
    * [.type](#Credentials+type) : <code>String</code>
    * [.username](#Credentials+username) : <code>String</code> &#124; <code>undefined</code>
    * [.getValue(property)](#Credentials+getValue) ⇒ <code>\*</code> &#124; <code>undefined</code>
    * [.getValueOrFail(property)](#Credentials+getValueOrFail) ⇒ <code>\*</code>
    * [.setValue(property, value)](#Credentials+setValue) ⇒ <code>[Credentials](#Credentials)</code>

<a name="Credentials+password"></a>

### credentials.password : <code>String</code> &#124; <code>undefined</code>
The password

**Kind**: instance property of <code>[Credentials](#Credentials)</code>  
<a name="Credentials+type"></a>

### credentials.type : <code>String</code>
The credentials type

**Kind**: instance property of <code>[Credentials](#Credentials)</code>  
**Read only**: true  
<a name="Credentials+username"></a>

### credentials.username : <code>String</code> &#124; <code>undefined</code>
The username

**Kind**: instance property of <code>[Credentials](#Credentials)</code>  
<a name="Credentials+getValue"></a>

### credentials.getValue(property) ⇒ <code>\*</code> &#124; <code>undefined</code>
Get a value from the credentials

**Kind**: instance method of <code>[Credentials](#Credentials)</code>  
**Returns**: <code>\*</code> &#124; <code>undefined</code> - Returns the value if found, or undefined  

| Param | Type | Description |
| --- | --- | --- |
| property | <code>String</code> | The property to fetch |

<a name="Credentials+getValueOrFail"></a>

### credentials.getValueOrFail(property) ⇒ <code>\*</code>
Get a value, or fail if it doesn't exist or isn't set

**Kind**: instance method of <code>[Credentials](#Credentials)</code>  
**Returns**: <code>\*</code> - The value (not undefined)  
**Throws**:

- <code>Error</code> Throws if the value is undefined


| Param | Type | Description |
| --- | --- | --- |
| property | <code>String</code> | The property to fetch |

<a name="Credentials+setValue"></a>

### credentials.setValue(property, value) ⇒ <code>[Credentials](#Credentials)</code>
Set a value for a property

**Kind**: instance method of <code>[Credentials](#Credentials)</code>  
**Returns**: <code>[Credentials](#Credentials)</code> - Returns self, for chaining  

| Param | Type | Description |
| --- | --- | --- |
| property | <code>String</code> | The property to set |
| value | <code>\*</code> | The value to set for the property |

<a name="EntryFacade"></a>

## EntryFacade : <code>Object</code>
Entry facade for data input

**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| type | <code>String</code> | The type of the facade |
| fields | <code>[Array.&lt;EntryFacadeField&gt;](#EntryFacadeField)</code> | An array of fields |

<a name="EntryFacadeField"></a>

## EntryFacadeField : <code>Object</code>
Entry facade data field

**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| title | <code>String</code> | The user-friendly title of the field |
| field | <code>String</code> | The type of data to map back to on the Entry instance (property/meta/attribute) |
| property | <code>String</code> | The property name within the field type of the Entry instance |
| value | <code>String</code> | The value of the property (read/write) |
| secret | <code>Boolean</code> | Wether or not the value should be hidden while viewing (masked) |
| multiline | <code>Boolean</code> | Whether the value should be edited as a multiline value or not |
| formatting | <code>Object</code> &#124; <code>Boolean</code> | Vendor formatting options object, or false if no formatting necessary |
| maxLength | <code>Number</code> | Maximum recommended length of the value (defaults to -1) |

<a name="FoundGroupResult"></a>

## FoundGroupResult : <code>Object</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| group | <code>Object</code> | The found group dataset |
| index | <code>Number</code> | The index the group was located at |

