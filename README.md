[P1_230211206_Yudha.json](https://github.com/user-attachments/files/34739150/P1_230211206_Yudha.json)# GDGoC-n8n-StudyJam
Kumpulan tugas dan alur kerja otomasi n8n AI Study Jam GDGoC Universitas Widyatama
GDGoC-n8n-StudyJam/
├── README.md
├── Pertemuan-01/
│   ├── P1_Nama.json
[Uploadi{
  "name": "My workflow",
  "nodes": [
    {
      "parameters": {
        "httpMethod": "POST",
        "path": "P1-Test",
        "responseMode": "responseNode",
        "options": {}
      },
      "type": "n8n-nodes-base.webhook",
      "typeVersion": 2.2,
      "position": [
        0,
        0
      ],
      "id": "018b8c0e-4151-41af-875a-bb170bc536df",
      "name": "Webhook",
      "webhookId": "80994085-217f-470e-a07a-4bb889bed2a4"
    },
    {
      "parameters": {
        "assignments": {
          "assignments": [
            {
              "id": "076bc403-3f76-4c5f-98c6-73d7dc9d4eab",
              "name": "Status",
              "value": "Succes",
              "type": "string"
            },
            {
              "id": "fc9942c1-6b82-4d8d-bf5d-4f0dcbbb99e7",
              "name": "Message",
              "value": "=Terimakasih {{$json.body.nama}} Pesan Kamu {{ $json.body.Pesan }}",
              "type": "string"
            }
          ]
        },
        "options": {}
      },
      "type": "n8n-nodes-base.set",
      "typeVersion": 3.5,
      "position": [
        224,
        0
      ],
      "id": "953bbac8-7a26-4310-b41c-173417f48ffa",
      "name": "Edit Fields"
    },
    {
      "parameters": {
        "options": {}
      },
      "type": "n8n-nodes-base.respondToWebhook",
      "typeVersion": 1.5,
      "position": [
        448,
        0
      ],
      "id": "b5bf2bc1-add1-4cc4-af58-9eee0ca4adfc",
      "name": "Respond to Webhook"
    }
  ],
  "pinData": {},
  "connections": {
    "Webhook": {
      "main": [
        [
          {
            "node": "Edit Fields",
            "type": "main",
            "index": 0
          }
        ]
      ]
    },
    "Edit Fields": {
      "main": [
        [
          {
            "node": "Respond to Webhook",
            "type": "main",
            "index": 0
          }
        ]
      ]
    }
  },
  "active": false,
  "settings": {
    "executionOrder": "v1",
    "binaryMode": "separate"
  },
  "versionId": "4dff596c-2dc9-480a-a401-16cd754b12c0",
  "meta": {
    "instanceId": "a8a592fa6ef200d26a624b2d178a8f1e3626b3be2ffd120cddf5c92642ae3e2b"
  },
  "nodeGroups": [],
  "id": "U9NjvPGGUeustQhP",
  "tags": []
}ng P1_230211206_Yudha.json…]()

│   └── P1_Nama.png 
<img width="511" height="351" alt="P1 (Hoppscotch)_230211206_Yudha" src="https://github.com/user-attachments/assets/eaf3bbf6-9730-411a-b5f3-2caeb243ae34" /> 
<img width="832" height="464" alt="P1 (Canvas)_230211206_Yudha" src="https://github.com/user-attachments/assets/a50e568e-8234-4eb1-8565-392db47037f9" />
├── Pertemuan-02/
│   ├── P2_Nama.json
│   └── P2_Nama.png
├── Pertemuan-03/
│   ├── P3_Nama.json
│   └── P3_Nama.png
├── Pertemuan-04/
│   ├── P4_Nama.json
│   └── P4_Nama.png
└── Pertemuan-05/
    ├── P5_Nama.json
    └── P5_Nama.png
