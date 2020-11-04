Вы должны отправлять файлы в таком формате:
### Пример:
```yml
# Предметы в обычных сундуках(стоят по всей карте)
items:
- STONE_SWORD 1 x:5
- GOLDEN_SWORD 1
- MUSHROOM_STEW 1 x:2
- STONE_HOE 1
- LEATHER_HELMET 1 x:2
- LEATHER_CHESTPLATE 1 x:2
- LEATHER_LEGGINGS 1 x:2
- IRON_HELMET 1 x:2
- IRON_CHESTPLATE 1 x:2
- IRON_LEGGINGS 1 x:2
- IRON_BOOTS 1 x:2
- BOW 1 x:3
- ARROW 20 x:2
- MILK_BUCKET 1 x:2
- FISHING_ROD 1
- COMPASS 1
- STICK 1 name:&6TrackingStick_&aUses:_5
- GOLDEN_HELMET 1
- GOLDEN_CHESTPLATE 1
- BONE 1 x:2
- GOLDEN_LEGGINGS 1
- GOLDEN_BOOTS 1
- DIAMOND_SWORD 1 name:&6Death_Dealer
- GOLDEN_APPLE 1
- CHAINMAIL_CHESTPLATE 1 x:1
- CHAINMAIL_LEGGINGS 1 x:1
- COOKIE 2 x:3
- MELON_SLICE 1 x:4
- COOKED_BEEF 1 x:2
- ENDER_PEARL 1 x:2
- POTION potion:SPEED:3600:1 1 x:2
- POTION potion:HEAL:1:1 1 x:2
- SPLASH_POTION potion:POISON:320:2 1
- SPLASH_POTION potion:REGENERATION:660:1 1 x:2
- APPLE 2 x:5
# Бонусные сундуки(бочки, шалкер-боксы, сундуки-ловушки, стоят на спавне и в труднодоступных местах)
bonus:
- DIAMOND_SWORD 1 enchant:sharpness:5 name:&3Power_Sword
- DIAMOND_CHESTPLATE 1 enchant:protection:3 name:&aLife_Saver
```
### Предметы:
Вы должны писать предметы в таком формате:<br>
\- ITEM_NAME STACK_SIZE x:CHANCE *другие параметры*
- `ITEM_NAME` - название предмета в соответсвии с SpigotAPI, список вы можете найти **[здесь](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html)**
- `STACK_SIZE` - количество предметов, генерируемых в одном слоте.
- `CHANCE` - шанс выпадения предмета. По умолчанию 1
#### Другие параметры:
- `name:` - имя, которое будет дано предмету при генерации. Пример: `name:&6Покупайте деньги`
- `lore:` - лор предмета. Пример: `lore:&7Jebaited`
- `enchant:` - зачарования предмета. Пример: `enchant:sharpness:2`
- `color:` - цвет предмета в десятичном формате. Пример: `color:1213666`
- `data:` - NBT дата предмета, в формате майнкрафта. Пример: `data:{StoredEnchantments:[{id:"minecraft:punch",lvl:2s}]}`
####Параметры зелий:
Параметры зелий - параметр к предмету в таком формате: `potion:EFFECT_TYPE:DURATION:AMPLIFIER`
- Возможные предметы, на которые работают данные параметры: `POTION`,`SPLASH_POTION`,`LINGERING_POTION`,`TIPPED_ARROW`
- `EFFECT_TYPE` - тип эффекта, вы можете использовать [названия зелий от Bukkit](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/potion/PotionEffectType.html) или [стандартные названия майнкрафта](https://minecraft.gamepedia.com/Status_effect#Effect_IDs)
- `DURATION` - длительность эффекта в секундах.
- `AMPLIFIER` - уровень эффекта(2 для силы 2 и т.д.)
- Если вы хотите несколько эффектов, то вам надо разделить их точкой с запятой `;`. Пример: `potion:HEAL:60:2;LUCK:50:1`
