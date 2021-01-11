CONTENTS OF THIS FILE
---------------------

 * Introduction
 * Webhook Data Request

INTRODUCTION
------------

All Webhook of Omni Agent
   
Webhook Data Request
------------

1: LivechatSessionStart

```bash
{
    "_id": "string",
    "label": "string",
    "createdAt": "2021-01-11T01:49:36.032Z",
    "lastMessageAt": "2021-01-11T01:49:36.032Z",
    "visitor": {
        "_id": "B5aW2A2bqzCPRRmk8",
        "token": "tranminhthan1111111gdauxanh555",
        "name": "string",
        "username": "string",
        "email": [
            {
                "address": "string"
            }
        ],
        "phone": [
            {
                "phoneNumber": "55 51 5555-55355"
            }
        ]
    },
    "type": "LivechatSessionStart",
    "messages": []
}
```


2: LivechatSessionTaken

```bash
{
    "_id": "string",
    "label": "string",
    "createdAt": "2021-01-11T01:49:36.032Z",
    "lastMessageAt": "2021-01-11T01:49:36.032Z",
    "visitor": {
        "_id": "B5aW2A2bqzCPRRmk8",
        "token": "tranminhthan1111111gdauxanh555",
        "name": "string",
        "username": "string",
        "email": [
            {
                "address": "string"
            }
        ],
        "phone": [
            {
                "phoneNumber": "string"
            }
        ]
    },
    "agent": {
        "_id": "string",
        "username": "string",
        "name": "string",
        "email": "string"
    },
    "type": "LivechatSessionTaken",
    "messages": [],
    "departmentId": "9MCmpkXDqKcwouqrT",
    "servedBy": {
        "_id": "string",
        "username": "string",
        "ts": "2021-01-11T01:49:36.190Z"
    }
}
```

3: Message (customer sending)

```bash
{
    "_id": "9etoLPY5JY2gCxBaC",
    "label": "string",
    "createdAt": "2021-01-11T01:49:36.032Z",
    "lastMessageAt": "2021-01-11T01:49:36.032Z",
    "visitor": {
        "_id": "B5aW2A2bqzCPRRmk8",
        "token": "tranminhthan1111111gdauxanh555",
        "name": "string",
        "username": "string",
        "email": [
            {
                "address": "string"
            }
        ],
        "phone": [
            {
                "phoneNumber": "string"
            }
        ]
    },
    "agent": {
        "_id": "string",
        "username": "string",
        "name": "string",
        "email": "string"
    },
    "type": "Message",
    "messages": [
        {
            "u": {
                "_id": "B5aW2A2bqzCPRRmk8",
                "username": "guest-87",
                "name": "Thang test LiveChat 2"
            },
            "_id": "GcH4xwp8LCpdqGmgp",
            "username": "guest-87",
            "msg": "sending livechat message..",
            "ts": "2021-01-11T02:01:46.186Z"
        }
    ]
}
```

4: Message (Agent sending)
```bash
{
    "_id": "string",
    "label": "string",
    "createdAt": "2021-01-11T01:49:36.032Z",
    "lastMessageAt": "2021-01-11T02:01:46.186Z",
    "visitor": {
        "_id": "B5aW2A2bqzCPRRmk8",
        "token": "tranminhthan1111111gdauxanh555",
        "name": "string",
        "username": "string",
        "email": [
            {
                "address": "string"
            }
        ],
        "phone": [
            {
                "phoneNumber": "string"
            }
        ]
    },
    "agent": {
        "_id": "string",
        "username": "string",
        "name": "string",
        "email": "string"
    },
    "type": "Message",
    "messages": [
        {
            "u": {
                "_id": "string",
                "username": "string",
                "name": "string"
            },
            "_id": "Btfc6y5WkjMZXi7Jj",
            "username": "string",
            "msg": "hi",
            "ts": "2021-01-11T02:03:20.872Z",
            "agentId": "BXpTEyaGjJu7nDMBG"
        }
    ]
}
```

5. LivechatSessionForwarded

```bash
{
    "_id": "9etoLPY5JY2gCxBaC",
    "label": "Thang test LiveChat 2",
    "createdAt": "2021-01-11T01:49:36.032Z",
    "lastMessageAt": "2021-01-11T02:03:20.872Z",
    "visitor": {
        "_id": "B5aW2A2bqzCPRRmk8",
        "token": "tranminhthan1111111gdauxanh555",
        "name": "Thang test LiveChat 2",
        "username": "guest-87",
        "email": [
            {
                "address": "visitor@rocket.cha3t"
            }
        ],
        "phone": [
            {
                "phoneNumber": "55 51 5555-55355"
            }
        ]
    },
    "agent": {
        "_id": "mYBoZL7dqaMc7GXQv",
        "username": "thangtm",
        "name": "Tran Minh Thang",
        "email": "thangtm@fpt.com.vn"
    },
    "type": "LivechatSessionForwarded",
    "messages": [
        {
            "u": {
                "_id": "B5aW2A2bqzCPRRmk8",
                "username": "guest-87",
                "name": "Thang test LiveChat 2"
            },
            "_id": "GcH4xwp8LCpdqGmgp",
            "username": "guest-87",
            "msg": "sending livechat message..",
            "ts": "2021-01-11T02:01:46.186Z"
        },
        {
            "u": {
                "_id": "string",
                "username": "string",
                "name": "string"
            },
            "_id": "string",
            "username": "string",
            "msg": "hi",
            "ts": "2021-01-11T02:03:20.872Z",
            "agentId": "BXpTEyaGjJu7nDMBG"
        }
    ],
    "departmentId": "9MCmpkXDqKcwouqrT",
    "servedBy": {
        "_id": "mYBoZL7dqaMc7GXQv",
        "username": "thangtm",
        "ts": "2021-01-11T02:16:29.388Z"
    },
    "oldServedBy": {
        "_id": "BXpTEyaGjJu7nDMBG",
        "username": "string",
        "ts": "2021-01-11T01:49:36.190Z"
    }
}
```

6. LivechatSession Close Room

```bash
{
    "_id": "9etoLPY5JY2gCxBaC",
    "label": "Thang test LiveChat 2",
    "createdAt": "2021-01-11T01:49:36.032Z",
    "lastMessageAt": "2021-01-11T02:03:20.872Z",
    "tags": [],
    "visitor": {
        "_id": "B5aW2A2bqzCPRRmk8",
        "token": "tranminhthan1111111gdauxanh555",
        "name": "Thang test LiveChat 2",
        "username": "guest-87",
        "email": [
            {
                "address": "visitor@rocket.cha3t"
            }
        ],
        "phone": [
            {
                "phoneNumber": "55 51 5555-55355"
            }
        ]
    },
    "agent": {
        "_id": "mYBoZL7dqaMc7GXQv",
        "username": "thangtm",
        "name": "Tran Minh Thang",
        "email": "thangtm@fpt.com.vn"
    },
    "type": "LivechatSession",
    "messages": [
        {
            "u": {
                "_id": "B5aW2A2bqzCPRRmk8",
                "username": "guest-87",
                "name": "Thang test LiveChat 2"
            },
            "_id": "GcH4xwp8LCpdqGmgp",
            "username": "guest-87",
            "msg": "sending livechat message..",
            "ts": "2021-01-11T02:01:46.186Z"
        },
        {
            "u": {
                "_id": "BXpTEyaGjJu7nDMBG",
                "username": "string",
                "name": "string"
            },
            "_id": "Btfc6y5WkjMZXi7Jj",
            "username": "string",
            "msg": "hi",
            "ts": "2021-01-11T02:03:20.872Z",
            "agentId": "BXpTEyaGjJu7nDMBG"
        },
        {
            "u": {
                "_id": "mYBoZL7dqaMc7GXQv",
                "username": "thangtm",
                "name": "Tran Minh Thang"
            },
            "_id": "9nQvHaCLg6kxCGkLX",
            "username": "thangtm",
            "msg": "99999999",
            "ts": "2021-01-11T02:22:05.372Z",
            "agentId": "mYBoZL7dqaMc7GXQv",
            "closingMessage": true
        }
    ],
    "departmentId": "9MCmpkXDqKcwouqrT",
    "servedBy": {
        "_id": "mYBoZL7dqaMc7GXQv",
        "username": "thangtm",
        "ts": "2021-01-11T02:16:29.388Z"
    },
    "closedAt": "2021-01-11T02:22:05.179Z",
    "closedBy": {
        "_id": "mYBoZL7dqaMc7GXQv",
        "username": "thangtm"
    },
    "closer": "user"
}
```
