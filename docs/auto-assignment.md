---
id: auto-assignment
title: How to setup round robin/automatic chats assignment workflow?
sidebar_label: Auto assignment
---

### Precondition

To user explicitly has to be assigned department. It's not enough just check all departments. Within each department have to be checked department.

### Department adjustment

You have in department "Auto assignment" secion enable automatic chats transfer.

*   Also optionally you can setup how many active chats user can have at a time.
*   How long chat should be assigned to user before it will be transfered to another user, if first user did not accepted it.
*   In most cases it's enough just enable enable it. I also recommend to read round robin implementation for chat's [https://docs.google.com/file/d/0B5uaj1QNYoNTVjRnd1ozdmJDYlkwMEl0T0p6NnZLeThXeEww/edit](https://docs.google.com/file/d/0B5uaj1QNYoNTVjRnd1ozdmJDYlkwMEl0T0p6NnZLeThXeEww/edit)

### Users adjustment

By default users sees all pending department chats. To disable that and show only to him assigned pending chats you have to

*   Edit user and in "Pending chats" tab, uncheck "User can see all pending chats, not only assigned to him"
*   By default operators do not have permission to choose what pending chats they can see. You can grant permission to choose them personally what list he want's to see. Assigned to operators role permission
*   "lhuser" => "allowtochoosependingmode" | "Users, groups management" => "Allow user to choose what pending chats he can see, only assigned to him or all."
*   User has to be online for chat being assigned to him
*   If you want that assigned chat would be opened automatically for user. User in his account has have checked "Chats" => "Automatically accept assigned chats"
    *   If user does not see Chats tab in his account you have to give operators role this permission Module - (lhuser) Function - (allowtochoosependingmode)
*   Also in "Visible lists" worh checking "My pending and active chats list enabled" so user would see new widget where only to him assigned active and pending chats would be presented. For user to be able to change what he sees he has to have this permission
    *   Module - ('lhuser'), Function - ('change_visibility_list')

<iframe width="560" height="315" src="https://www.youtube.com/embed/4PTkaAs452A" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>