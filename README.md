sgs-octgn
=========

OCTGN Game Definition for 三国杀阵面对决

OCTGN脚本基于mtg-octgn开发。目前没有多少改动。The game definition itself is based on [brine's mtg-octgn project](https://github.com/brine/mtg-octgn) with very little change.

## 安装 Installation
将definition目录下的`.nupkg`文件复制到OCTGN/LocalFeed目录下。在OCTGN的游戏管理中安装。

Copy the `.nupkg` file into OCTGN LocalFeed directory. Then you can find the game in OCTGN>GameManager>LocalFeed

## 卡牌图片 Card Image
卡牌图片文件位于card_image_pack目录下。

Install the file under card_image_pack directory.

## 使用手册

### 游戏准备

1. 载入套牌：Game->Load Deck (`ctrl+l`)
2. 抽起始手牌：右键选择手牌区->抽起始手牌
3. 手牌调度：
	1. `shift` +鼠标左键选择本次需要调度的所有手牌
	2. 右键选择手牌区->调度选择的手牌(`ctrl+m`)
	3. 重复i，ii直到不再需要调度
	3. 右键选择牌库->洗牌

### 游戏功能说明 Explanation of some game functions

#### OCTGN自带功能 UNIVERSAL OCTGN FUNCTIONS (not linked to game functions)

(这些功能在所有OCTGN游戏中均可使用 these work in ALL OCTGN games, not just SGS)

* 放大牌局 Zoom the Table
-- 鼠标滚轮 Use the scroll wheel on a mouse.
* 移动牌局 Move/Pan the Table
-- 按住空格并拖拽牌局 Hold the spacebar and click-drag the Table.
* 放置/移除卡牌标记物 Increment/Decrement counters on a card
-- Use the +/- keys on your keyboard's NUM pad while hovering over the counter.
* 将标记物移动到另一张卡上 Move counters from one card to another
-- 点击拖拽标记物 Click-drag the counter to the other card.
* 选择/取消目标 Target/untarget a card
-- `shift` +鼠标左键 Hold SHIFT and click on the card.
* 在卡牌之间画箭头 draw an Arrow between two cards
-- `shift` +点击拖拽 Hold SHIFT and click-drag from one card to the other.
* 选择多张卡牌 Select multiple cards
-- 鼠标画框范围选择或`ctrl` +鼠标左键 Either click-drag a selection box over the region of cards, or hold CTRL and click a card.
* 暗置手牌进场 Play card face-down from your hand
-- 拖拽卡牌在放下前按住`shift` Click-Drag a card in your hand, then hold SHIFT as you drop the card onto the Table.


#### 阵面对决牌桌功能 SGS-SPECIFIC TABLE FUNCTIONS
* 将卡牌附属于目标卡 Attach/Equip/Bond a card to another card (CTRL+Q)
-- 选择目标被附属卡 Target (shift-click) the card that will be the 'target' of the attachment.
-- `ctrl+Q`或右键选择“附属于目标卡” Right-click the Attachment card (Equipment/Aura, etc) and select "Attach to Targeted Card" (or use the CTRL+Q shortcut).
* 取消附属 Detaching a card (CTRL+Q)
-- 在已附属卡牌上使用附属于目标卡（`ctrl+Q`）功能 Using the "Attach to Targeted Card" (CTRL+Q) action on a card that is already attached to something else will detach that card from everything it's attached to.
* 将卡牌翻面 Flip Card (CTRL+F)
-- 将地牌翻面或翻回。
* 将卡牌已随机顺序置于牌库底 Shuffle Cards to Bottom of Library
* 检查卡牌说明 Check Card Rulings (on iplaysgs.com)
-- 打开营地卡查连接 Will open up your internet browser and link you to the card's iplaysgs.com page

#### 阵面对决手牌功能 SGS-SPECIFIC HAND FUNCTIONS
* 占星 Scry (CTRL+SHIFT+C)
-- 更快结算占星异能 Allows you to resolve scry triggers faster than manually viewing the top X cards of your deck.
-- 第一个对话框提问需要抓多少牌。输入牌数并确定。The first box asks how much you wish to scry for.  Enter the scry value and press OK.
-- 新对话框会展示你占星的所有牌。A new box will pop up with a list of buttons for each card you are scrying.
-- 按`Switch to TOP/BOTTOM`选择卡牌放置位置。To add cards to the TOP of your deck (or switch back to BOTTOM), click the 'Switch to TOP' or 'Switch to BOTTOM' button on the bottom.
-- 按带有卡名的按钮将牌置于牌库顶/底。To add a card to the BOTTOM of your deck, click the button with the card name.
-- 牌库在所有操作完成前不会被改动，占星过程可随时取消并重新开始。The scry function will not rearrange your deck until all cards have been selected.  Cancelling out at any time will cancel the scry without rearranging.

