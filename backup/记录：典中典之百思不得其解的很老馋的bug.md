再跟着godot的官方文档学着捣鼓那个”your first 2d game“，然后最后一步是加快捷键

<img width="461" height="85" alt="Image" src="https://github.com/user-attachments/assets/1c3ea540-317c-4eab-9724-9dee7507be93" />

<img width="540" height="410" alt="Image" src="https://github.com/user-attachments/assets/29ff1704-f75b-47a0-8238-f2c04f9b78ef" />

看起来好像非常正常，但是这个快捷键他就是不好使
然后我瞧了眼调试器，发现了这个报错：
E 0:00:02:910   event_get_action_status: The InputMap action "start_game" doesn't exist. Did you mean "start_game "?

然后我盯着这玩意盯了半天，把后面那个”start_game“直接复制下来塞进那个action里也不好使
给我干成智力障碍了

那么最后问题出在哪里呢？
我写在项目调整里那个action叫做”start_game “ 
把两个挑出来一对比就知道了，我这前面写项目调整里的这玩意多了个空格

总结：我是傻逼
