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
	1. `shift+`鼠标左键选择本次需要调度的所有手牌
	2. 右键选择手牌区->调度选择的手牌(`ctrl+m`)
	3. 重复i，ii直到不再需要调度
	3. 右键选择牌库->洗牌

