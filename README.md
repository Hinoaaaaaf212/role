# role

A command that adds the role to the mentioned user, if the user already has the role then it removes it from them.


Raw Data: ```{
    "name": "role",
    "permissions": "NONE",
    "restriction": "1",
    "_id": "lTaMQ",
    "actions": [
        {
            "info": "1",
            "infoIndex": "2",
            "storage": "1",
            "varName": "storeCommandParams",
            "name": "Store Command Params"
        },
        {
            "info": "1",
            "find": "${tempVars(\"storeCommandParams\")}",
            "storage": "1",
            "varName": "findRole",
            "name": "Find Role"
        },
        {
            "storage": "1",
            "varName": "findRole",
            "comparison": "0",
            "value": "",
            "iftrue": "0",
            "iftrueVal": "",
            "iffalse": "2",
            "iffalseVal": "13",
            "name": "Check Variable"
        },
        {
            "member": "0",
            "varName": "",
            "role": "3",
            "varName2": "findRole",
            "iftrue": "2",
            "iftrueVal": "21",
            "iffalse": "0",
            "iffalseVal": "",
            "name": "Check If Member has Role"
        },
        {
            "condition": "0",
            "comparison": "0",
            "value": "2",
            "iftrue": "0",
            "iftrueVal": "",
            "iffalse": "2",
            "iffalseVal": "19",
            "name": "Check Parameters"
        },
        {
            "server": "0",
            "varName": "",
            "storage": "1",
            "varName2": "getBotasMember",
            "name": "Get Bot as Member"
        },
        {
            "member": "2",
            "varName": "getBotasMember",
            "permission": "MANAGE_ROLES",
            "iftrue": "0",
            "iftrueVal": "",
            "iffalse": "2",
            "iffalseVal": "17",
            "name": "Check Member Permissions"
        },
        {
            "member": "1",
            "varName": "",
            "permission": "MANAGE_ROLES",
            "iftrue": "0",
            "iftrueVal": "",
            "iffalse": "2",
            "iffalseVal": "15",
            "name": "Check Member Permissions"
        },
        {
            "member": "0",
            "varName": "",
            "info": "18",
            "storage": "1",
            "varName2": "storeMemberInfo",
            "name": "Store Member Info"
        },
        {
            "member": "0",
            "varName2": "",
            "role": "3",
            "varName": "findRole",
            "name": "Add Member Role"
        },
        {
            "channel": "0",
            "varName": "",
            "message": "Added ${tempVars(\"findRole\")} to ${tempVars(\"storeMemberInfo\")} succesfully!",
            "storage": "0",
            "varName2": "",
            "iffalse": "0",
            "iffalseVal": "",
            "name": "Send Message"
        },
        {
            "name": "End Action Sequence"
        },
        {
            "channel": "0",
            "varName": "",
            "message": "Error: Please make sure the role you are trying to add to the target user exists.",
            "storage": "0",
            "varName2": "",
            "iffalse": "0",
            "iffalseVal": "",
            "name": "Send Message"
        },
        {
            "name": "End Action Sequence"
        },
        {
            "channel": "0",
            "varName": "",
            "message": "Error: You need the required permissions to use this command:\n\nManage Roles",
            "storage": "0",
            "varName2": "",
            "iffalse": "0",
            "iffalseVal": "",
            "name": "Send Message"
        },
        {
            "name": "End Action Sequence"
        },
        {
            "channel": "0",
            "varName": "",
            "message": "Error: The bot needs the following permissions to role the targeted member:\n\nManage Roles",
            "storage": "0",
            "varName2": "",
            "iffalse": "0",
            "iffalseVal": "",
            "name": "Send Message"
        },
        {
            "name": "End Action Sequence"
        },
        {
            "channel": "0",
            "varName": "",
            "message": "Error: Please put the correct usage for to role a member.\n\nExample: [p]role ${member} Bot Maker",
            "storage": "0",
            "varName2": "",
            "iffalse": "0",
            "iffalseVal": "",
            "name": "Send Message"
        },
        {
            "name": "End Action Sequence"
        },
        {
            "member": "0",
            "varName2": "",
            "role": "3",
            "varName": "findRole",
            "name": "Remove Member Role"
        },
        {
            "member": "0",
            "varName": "",
            "info": "18",
            "storage": "1",
            "varName2": "storeMemberInfo2",
            "name": "Store Member Info"
        },
        {
            "channel": "0",
            "varName": "",
            "message": "Removed ${tempVars(\"findRole\")} from ${tempVars(\"storeMemberInfo2\")} succesfully!",
            "storage": "0",
            "varName2": "",
            "iffalse": "0",
            "iffalseVal": "",
            "name": "Send Message"
        }
    ]
}```
