# Minecraft MakeCode 教學：幫助奇怪的巫師完成祭典

## Step 1：先做聊天開關

先放聊天積木。
按下「T」或是「Enter」在聊天室中打 「run」。
程式才會動起來。

```blocks
player.onChat("run", function () {

})
```

---

## Step 2：認識世界座標 world()
世界裡每一個地方都有住址。
world(數字, 數字, 數字) 就是位置。
試著把自己傳送到以下位置(525, -60, 500)

```blocks
player.onChat("1", function () {
    player.teleport(world(525, -60, 500))
})
```

---

## Step 3：在指定位置放一張床
現在要真的放東西了。
BED 是床。
blocks.place 是放方塊。
world(515, -58, 505) 是巫師指定的位置。
聊天打 run。
你會看到一張床出現。

```blocks
player.onChat("run", function () {
    blocks.place(BED, world(515, -58, 505))
})
```

---

## Step 4：再放一張床在旁邊
祭典需要兩張床。
再加一個放床的積木。
位置改成 world(514, -58, 505)。
這個位置就在旁邊。
聊天打 run。
你會看到第二張床。

```blocks
player.onChat("run", function () {
    blocks.place(BED, world(515, -58, 505))
    blocks.place(BED, world(514, -58, 505))
})
```

---

## Step 5：確認床的位置
現在兩張床都放好了。
它們在同一個高度。
只是左右位置不同。
畫面上可以清楚看到兩張床。
祭典準備已經快完成了。

```blocks
player.onChat("run", function () {
    blocks.place(BED, world(515, -58, 505))
    blocks.place(BED, world(514, -58, 505))
})
```

---

## Step 6：完成巫師的祭典程式
這就是完整的儀式程式。
聊天輸入 run。
兩張床會出現在指定位置。
巫師的祭典完成了。
你成功幫上忙了。

```blocks
player.onChat("run", function () {
    blocks.place(BED, world(515, -58, 505))
    blocks.place(BED, world(514, -58, 505))
})
```