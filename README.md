# ERPImport
一个简易关于数据库与visual studio联合建立成ERP系统的项目，现只是读取Excel阶段
流程
导入流程：
Excel
↓
Provider（提供的接口）
↓
Validator（校检）
↓
DataTable（数据）
↓
BulkCopy（复制到临时表）
↓
Merge（同步）
↓
History（历史记录）
↓
Email（邮件发送，看完成情况）
↓
Backup（备份）

sql：job流程
SQL Job
↓
Console（控制台自动导入部分）
↓
ProductImportService（窗体与控制台共用）
↓
Database（数据库）
完全的
ERPImport
│
├── ERPImport.WinForm
│
├── ERPImport.Console
│
├── ERPImport
│   ├── BLL
│   ├── DAL
│   ├── Models
│   ├── Providers
│   ├── Interfaces
│   ├── Factory
│   ├── Validators
│   ├── Utils
│   ├── Config
│   └── Common
│
├── Database
│
├── Docs
│
├── README.md
│
└── LICENSE
