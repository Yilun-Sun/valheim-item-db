# Valheim Item Database in .json

Remove unnecessary data and strip 'm_' at the beginning of each key.

## From
```yaml
MonoBehaviour:
  m_CorrespondingSourceObject: {fileID: 0}
  m_PrefabInstance: {fileID: 100100000}
  m_PrefabAsset: {fileID: 0}
  m_GameObject: {fileID: 1451307590010271}
  m_Enabled: 1
  m_EditorHideFlags: 0
  m_Script: {fileID: 11500000, guid: b3becef3e8ef1c54bb2f89618c36ae56, type: 3}
  m_Name:
  m_EditorClassIdentifier:
  m_autoPickup: 1
  m_autoDestroy: 1
  m_itemData:
    m_stack: 1
    m_durability: 100
    m_quality: 1
    m_variant: 0
    m_shared:
      m_name: $item_amber
      m_dlc:
      m_itemType: 1
      m_icons:
      - {fileID: 21300412, guid: 9c542d481b3563b4ab975314735bb3da, type: 3}
      m_attachOverride: 0
      m_description: $item_amber_description
      m_maxStackSize: 20
      m_maxQuality: 1
      m_weight: 0.1
      m_value: 5
      m_teleportable: 1
```

↓

↓

↓

## To
```json
"11480223484521100": {
    "_id": 11480223484521100,
    "Name": "Amber",
    "itemData": {
      "name": "$item_amber",
      "dlc": null,
      "itemType": 1,
      "attachOverride": 0,
      "description": "$item_amber_description",
      "maxStackSize": 20,
      "maxQuality": 1,
      "weight": 0.1,
      "value": 5,
      "teleportable": 1,
```

You will need `_id` in the recipes.