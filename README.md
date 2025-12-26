# exports-fo-ox_inventory
frequently used

```lua
# 获取物品名称
local function GetAllItemNames()
    local itemsTable = exports.ox_inventory:Items()
    local itemNames = {}
    
    if itemsTable then
        for itemName, _ in pairs(itemsTable) do
            table.insert(itemNames, itemName)
        end
        table.sort(itemNames) -- 按字母排序
    end
    
    return itemNames
end
```
