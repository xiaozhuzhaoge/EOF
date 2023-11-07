
# 命运挽歌创意工坊头像替换工具

1. 下载SteamMOD文件夹，并将其放在某个盘的根目录。只需要修改以下几个地方就可以创建自己的头像集合了:

2. 确保自己拥有《命运挽歌》游戏，这一步最重要，否则无法上传到创意工坊.

3. 主要修改Sample文件夹下的文件，ModPackage文件无需修改。打开Sample文件夹，可以看到3个文件夹以及2个文件:

   - images文件夹
   - paks文件夹
   - source文件夹
   - mod.vdf文件
   - mod_upload.bat文件

4. 在对头像进行修改并且上传之前，请将mod.vdf用记事本文件打开。会看到以下内容:

```markdown
"workshopitem"
{
	"appid"		"2191710"
	"contentfolder"		"D:\\SteamMOD\\Sample\\paks"
	"previewfile"		"D:\\SteamMOD\\Sample\\images\\f1.png"
	"visibility"		"0"
	"title"		"标题"
	"description"		"描述"
	"changenote"		"1.0"
	"publishedfileid"		""
}
```

需要修改的是：

- contentfolder 代表你的实际要上传的文件路径，请将paks所在的路径修改成当前你的盘符对应的路径。
- previewfile 代表你要上传的工坊mode道具的图片，路径修改为自己的文件夹路径。f1.png文件你可以在images文件夹中找到，使用PS自己做一个新的图片吧！
- 标题和描述可以自己写。

5. 接着使用记事本打开mod_upload.bat，可以看到以下文本:

```markdown
D:\SteamMOD\ModPackage\steamcmd.exe +login <usename> <password> +workshop_build_item D:\SteamMOD\Sample\mod.vdf +quit
```

将 `<usename>` 与 `<password>` 替换成自己的Steam用户名和密码。`D:\SteamMOD\ModPackage\steamcmd.exe` 这个路径也需要替换成实际自己的路径.

6. 接着修改paks中文件夹内的图片，使用自己的图片替换即可。游戏中默认头像是0.png，如果你有大的立绘可以在头像图片所在的文件夹放入1.png用来描述大的立绘，游戏中显示图片时会优先选择1.png进行显示。案例可以看paks\Sprites\Cards\NewFace\B215文件夹中的示例，0.png代表头像，1.png代表大的立绘。

7. 上方的文件如果都修改成功，双击mod_upload.bat运行来激活Steam上传你自己的mod。

8. 如果上传成功，则可以在官方创意工坊中看到自己的mod物品。点击订阅，启动游戏即可下载自己的mod进行头像替换。


# Fate Overture Creative Workshop Avatar Replacement Tool

1. Download the SteamMOD folder and place it in the root directory of a drive. You only need to make a few changes to create your own collection of avatars:

2. Make sure you have the game "Fate Overture" as this is crucial for uploading to the creative workshop.

3. The main modifications will be in the Sample folder, and you don't need to change the ModPackage files. Open the Sample folder, and you will see three folders and two files:

   - images folder
   - paks folder
   - source folder
   - mod.vdf file
   - mod_upload.bat file

4. Before making modifications to avatars and uploading them, open the mod.vdf file with a text editor. You will see the following content:

```markdown
"workshopitem"
{
	"appid"		"2191710"
	"contentfolder"		"D:\\SteamMOD\\Sample\\paks"
	"previewfile"		"D:\\SteamMOD\\Sample\\images\\f1.png"
	"visibility"		"0"
	"title"		"Title"
	"description"		"Description"
	"changenote"		"1.0"
	"publishedfileid"		""
}
```

What needs to be modified are:

- `contentfolder`, which represents the actual path of the files you want to upload. Replace it with the path to your paks folder corresponding to your drive.
- `previewfile`, which represents the image for the workshop mod item you want to upload. Change the path to your own folder. You can find the f1.png file in the images folder. Consider creating a new image using Photoshop!
- You can write your own title and description.

5. Next, open the mod_upload.bat file with a text editor. You will see the following text:

```markdown
D:\SteamMOD\ModPackage\steamcmd.exe +login <username> <password> +workshop_build_item D:\SteamMOD\Sample\mod.vdf +quit
```

Replace `<username>` and `<password>` with your own Steam username and password. You should also replace `D:\SteamMOD\ModPackage\steamcmd.exe` with your actual file path.

6. After making these changes, you can replace the images in the paks folders with your own. The default avatar in the game is 0.png, and if you have a larger illustration, you can place a 1.png in the same folder to represent the larger artwork. The game will prioritize displaying 1.png when showing the images. You can refer to the example in the paks\Sprites\Cards\NewFace\B215 folder, where 0.png represents the avatar and 1.png represents the larger artwork.

7. If you have successfully modified the files above, double-click the mod_upload.bat file to activate the upload of your mod to Steam.

8. If the upload is successful, you can find your mod item in the official Creative Workshop. Click "Subscribe" and start the game to download and use your mod for avatar replacement.
