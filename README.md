#命运挽歌创意工坊头像替换工具
下载SteamMOD文件夹，并将其放在某个盘的根目录
只需要修改以下几个地方就可以创建自己的头像集合了
1.确保自己拥有《命运挽歌》游戏，这一步最重要，否则无法上传到创意工坊。
2.主要修改Sample文件夹下的文件，ModPackage文件无需修改
3.打开Sample文件夹，可以看到3个文件夹以及2个文件
   images文件夹
   paks文件夹
   source文件夹
   mod.vdf文件
   mod_upload.bat文件
4.在对头像进行修改并且上传之前，请将mod.vdf用记事本文件打开。
会看到以下内容
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

需要修改的是：
contentfolder 代表你的实际要上传的文件路径，请将paks所在的路径修改成当前你的盘符对应的路径
previewfile 代表你要上传的工坊mode道具的图片,路径修改为自己的文件夹路径。
f1.png文件你可以在images文件夹中找到，使用PS自己做一个新的图片吧！
标题和描述可以自己写

5.接着使用记事本打开mod_upload.bat
可以看到以下文本
D:\SteamMOD\ModPackage\steamcmd.exe +login <usename> <password> +workshop_build_item D:\SteamMOD\Sample\mod.vdf +quit
将<usename> 与 <password> 替换成自己的Steam用户名和密码
D:\SteamMOD\ModPackage\steamcmd.exe 这个路径也需要替换成实际自己的路径.

6.接着修改paks中文件夹内的图片，使用自己的图片替换即可。游戏中默认头像是0.png，如果你有大的立绘可以在头像图片所在的文件夹放入1.png用来描述大的立绘，游戏中显示图片时会优先选择1.png进行显示。
案例可以看paks\Sprites\Cards\NewFace\B215文件夹中的示例,0.png代表头像 1.png代表大的立绘

7.上方的文件如果都修改成功，双击mod_upload.bat运行来激活Steam上传你自己的mod
8.如果上传成功，则可以在官方创意工坊中看到自己的mod物品。点击订阅，启动游戏即可下载自己的mod进行头像替换。


# Fate Requiem Workshop Avatar Replacement Tool
Download the SteamMOD folder and place it at the root of a drive.
You only need to modify a few places to create your own avatar collection:
1. Make sure you own "Fate Requiem" in your Steam library; this step is crucial, or you won't be able to upload to the Steam Workshop.
2. Mainly modify the files under the "Sample" folder; there's no need to change the "ModPackage" files.
3. Open the "Sample" folder, where you will see three folders and two files:
   - images folder
   - paks folder
   - source folder
   - mod.vdf file
   - mod_upload.bat file
4. Before making changes to the avatars and uploading them, open the "mod.vdf" file with a text editor.
You will see the following content:
"workshopitem"
{
    "appid"        "2191710"
    "contentfolder"        "D:\\SteamMOD\\Sample\\paks"
    "previewfile"        "D:\\SteamMOD\\Sample\\images\\f1.png"
    "visibility"        "0"
    "title"        "Title"
    "description"        "Description"
    "changenote"        "1.0"
    "publishedfileid"        ""
}

You need to modify the following:
- contentfolder represents the actual path of the files you want to upload. Please change the path to correspond to your drive's path for the "paks" folder.
- previewfile represents the image of the workshop item you want to upload. Change the path to point to your own image file. The "f1.png" file can be found in the "images" folder. You can create a new image using Photoshop or another image editing tool.
- Title and Description can be written as you wish.

5. Next, open "mod_upload.bat" using a text editor. You will see the following text:
D:\SteamMOD\ModPackage\steamcmd.exe +login <username> <password> +workshop_build_item D:\SteamMOD\Sample\mod.vdf +quit
Replace <username> and <password> with your own Steam username and password.
The path "D:\SteamMOD\ModPackage\steamcmd.exe" also needs to be replaced with your actual path.

6. Then, modify the images in the folders within "paks." Simply replace them with your own images. The default avatar in the game is "0.png." If you have larger illustrations, you can place a "1.png" in the same folder to provide a larger image. The game will prioritize "1.png" for displaying when available.
An example can be seen in the "paks\Sprites\Cards\NewFace\B215" folder; "0.png" represents the avatar, and "1.png" represents the larger illustration.

7. If you've successfully made changes to all the mentioned files, double-click "mod_upload.bat" to run it and activate Steam's upload of your mod.
8. If the upload is successful, you will be able to see your mod item in the official Steam Workshop. Subscribe to it, start the game, and you can download your mod to replace your avatars.