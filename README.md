# Rust API client for firefly-iii

[![Crates.io](https://img.shields.io/crates/v/firefly-iii.svg?maxAge=2592000)](https://crates.io/crates/firefly-iii)
[![Documentation](https://docs.rs/firefly-iii/badge.svg)](https://docs.rs/firefly-iii)

This is the official documentation of the Firefly III API. You can find accompanying documentation on the website of Firefly III itself (see below). Please report any bugs or issues. This version of the API is live from version v4.7.9 and onwards. You may use the \"Authorize\" button to try the API below.

## Overview

This API client was generated by the [OpenAPI Generator](https://openapi-generator.tech) project.  By using the [openapi-spec](https://openapis.org) from a remote server, you can easily generate an API client.

- API version: 0.10.4
- Package version: 0.10.4
- Build package: org.openapitools.codegen.languages.RustClientCodegen
For more information, please visit [https://firefly-iii.org](https://firefly-iii.org)

## Installation

Put the package under your project folder and add the following to `Cargo.toml` under `[dependencies]`:

```
firefly-iii = "0.1.0-alpha.3"
```

## Documentation for API Endpoints

All URIs are relative to *https://demo.firefly-iii.org*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AboutApi* | [**get_about**](docs/AboutApi.md#get_about) | **GET** /api/v1/about | System information end point.
*AboutApi* | [**get_current_user**](docs/AboutApi.md#get_current_user) | **GET** /api/v1/about/user | Currently authenticated user endpoint.
*AccountsApi* | [**delete_account**](docs/AccountsApi.md#delete_account) | **DELETE** /api/v1/accounts/{id} | Permanently delete account.
*AccountsApi* | [**get_account**](docs/AccountsApi.md#get_account) | **GET** /api/v1/accounts/{id} | Get single account.
*AccountsApi* | [**list_account**](docs/AccountsApi.md#list_account) | **GET** /api/v1/accounts | List all accounts.
*AccountsApi* | [**list_piggy_bank_by_account**](docs/AccountsApi.md#list_piggy_bank_by_account) | **GET** /api/v1/accounts/{id}/piggy_banks | List all piggy banks related to the account.
*AccountsApi* | [**list_transaction_by_account**](docs/AccountsApi.md#list_transaction_by_account) | **GET** /api/v1/accounts/{id}/transactions | List all transactions related to the account.
*AccountsApi* | [**store_account**](docs/AccountsApi.md#store_account) | **POST** /api/v1/accounts | Create new account.
*AccountsApi* | [**update_account**](docs/AccountsApi.md#update_account) | **PUT** /api/v1/accounts/{id} | Update existing account.
*AttachmentsApi* | [**delete_attachment**](docs/AttachmentsApi.md#delete_attachment) | **DELETE** /api/v1/attachments/{id} | Delete an attachment.
*AttachmentsApi* | [**download_attachment**](docs/AttachmentsApi.md#download_attachment) | **GET** /api/v1/attachments/{id}/download | Download a single attachment.
*AttachmentsApi* | [**get_attachment**](docs/AttachmentsApi.md#get_attachment) | **GET** /api/v1/attachments/{id} | Get a single attachment.
*AttachmentsApi* | [**list_attachment**](docs/AttachmentsApi.md#list_attachment) | **GET** /api/v1/attachments | List all attachments.
*AttachmentsApi* | [**store_attachment**](docs/AttachmentsApi.md#store_attachment) | **POST** /api/v1/attachments | Store a new attachment.
*AttachmentsApi* | [**update_attachment**](docs/AttachmentsApi.md#update_attachment) | **PUT** /api/v1/attachments/{id} | Update existing attachment.
*AttachmentsApi* | [**upload_attachment**](docs/AttachmentsApi.md#upload_attachment) | **POST** /api/v1/attachments/{id}/upload | Upload an attachment.
*AvailableBudgetsApi* | [**delete_available_budget**](docs/AvailableBudgetsApi.md#delete_available_budget) | **DELETE** /api/v1/available_budgets/{id} | Delete an available budget.
*AvailableBudgetsApi* | [**get_available_budget**](docs/AvailableBudgetsApi.md#get_available_budget) | **GET** /api/v1/available_budgets/{id} | Get a single available budget.
*AvailableBudgetsApi* | [**list_available_budget**](docs/AvailableBudgetsApi.md#list_available_budget) | **GET** /api/v1/available_budgets | List all available budget amounts.
*AvailableBudgetsApi* | [**store_available_budget**](docs/AvailableBudgetsApi.md#store_available_budget) | **POST** /api/v1/available_budgets | Store a new available budget
*AvailableBudgetsApi* | [**update_available_budget**](docs/AvailableBudgetsApi.md#update_available_budget) | **PUT** /api/v1/available_budgets/{id} | Update existing available budget, to change for example the date range of the amount or the amount itself.
*BillsApi* | [**delete_bill**](docs/BillsApi.md#delete_bill) | **DELETE** /api/v1/bills/{id} | Delete a bill.
*BillsApi* | [**get_bill**](docs/BillsApi.md#get_bill) | **GET** /api/v1/bills/{id} | Get a single bill.
*BillsApi* | [**list_attachment_by_bill**](docs/BillsApi.md#list_attachment_by_bill) | **GET** /api/v1/bills/{id}/attachments | List all attachments uploaded to the bill.
*BillsApi* | [**list_bill**](docs/BillsApi.md#list_bill) | **GET** /api/v1/bills | List all bills.
*BillsApi* | [**list_rule_by_bill**](docs/BillsApi.md#list_rule_by_bill) | **GET** /api/v1/bills/{id}/rules | List all rules associated with the bill.
*BillsApi* | [**list_transaction_by_bill**](docs/BillsApi.md#list_transaction_by_bill) | **GET** /api/v1/bills/{id}/transactions | List all transactions associated with the  bill.
*BillsApi* | [**store_bill**](docs/BillsApi.md#store_bill) | **POST** /api/v1/bills | Store a new bill
*BillsApi* | [**update_bill**](docs/BillsApi.md#update_bill) | **PUT** /api/v1/bills/{id} | Update existing bill.
*BudgetsApi* | [**delete_budget**](docs/BudgetsApi.md#delete_budget) | **DELETE** /api/v1/budgets/{id} | Delete a budget.
*BudgetsApi* | [**delete_budget_limit**](docs/BudgetsApi.md#delete_budget_limit) | **DELETE** /api/v1/budgets/limits/{id} | Delete a budget limit.
*BudgetsApi* | [**get_budget**](docs/BudgetsApi.md#get_budget) | **GET** /api/v1/budgets/{id} | Get a single budget.
*BudgetsApi* | [**get_budget_limit**](docs/BudgetsApi.md#get_budget_limit) | **GET** /api/v1/budgets/limits/{id} | Get single budget limit.
*BudgetsApi* | [**list_budget**](docs/BudgetsApi.md#list_budget) | **GET** /api/v1/budgets | List all budgets.
*BudgetsApi* | [**list_budget_limit_by_budget**](docs/BudgetsApi.md#list_budget_limit_by_budget) | **GET** /api/v1/budgets/{id}/limits | Get all limits
*BudgetsApi* | [**list_transaction_by_budget**](docs/BudgetsApi.md#list_transaction_by_budget) | **GET** /api/v1/budgets/{id}/transactions | All transactions to a budget.
*BudgetsApi* | [**list_transaction_by_budget_limit**](docs/BudgetsApi.md#list_transaction_by_budget_limit) | **GET** /api/v1/budgets/limits/{id}/transactions | List all transactions by a budget limit ID.
*BudgetsApi* | [**store_budget**](docs/BudgetsApi.md#store_budget) | **POST** /api/v1/budgets | Store a new budget
*BudgetsApi* | [**store_budget_limit**](docs/BudgetsApi.md#store_budget_limit) | **POST** /api/v1/budgets/{id}/limits | Store new budget limit.
*BudgetsApi* | [**update_budget**](docs/BudgetsApi.md#update_budget) | **PUT** /api/v1/budgets/{id} | Update existing budget.
*BudgetsApi* | [**update_budget_limit**](docs/BudgetsApi.md#update_budget_limit) | **PUT** /api/v1/budgets/limits/{id} | Update existing budget limit.
*CategoriesApi* | [**delete_category**](docs/CategoriesApi.md#delete_category) | **DELETE** /api/v1/categories/{id} | Delete a category.
*CategoriesApi* | [**get_category**](docs/CategoriesApi.md#get_category) | **GET** /api/v1/categories/{id} | Get a single category.
*CategoriesApi* | [**list_category**](docs/CategoriesApi.md#list_category) | **GET** /api/v1/categories | List all categories.
*CategoriesApi* | [**list_transaction_by_category**](docs/CategoriesApi.md#list_transaction_by_category) | **GET** /api/v1/categories/{id}/transactions | List all transactions in a category.
*CategoriesApi* | [**store_category**](docs/CategoriesApi.md#store_category) | **POST** /api/v1/categories | Store a new category
*CategoriesApi* | [**update_category**](docs/CategoriesApi.md#update_category) | **PUT** /api/v1/categories/{id} | Update existing category.
*ChartsApi* | [**get_chart_ab_overview**](docs/ChartsApi.md#get_chart_ab_overview) | **GET** /api/v1/chart/ab/overview/{id} | Dashboard chart with an overview of the available budget.
*ChartsApi* | [**get_chart_account_expense**](docs/ChartsApi.md#get_chart_account_expense) | **GET** /api/v1/chart/account/expense | Dashboard chart with expense account balance information.
*ChartsApi* | [**get_chart_account_overview**](docs/ChartsApi.md#get_chart_account_overview) | **GET** /api/v1/chart/account/overview | Dashboard chart with asset account balance information.
*ChartsApi* | [**get_chart_account_revenue**](docs/ChartsApi.md#get_chart_account_revenue) | **GET** /api/v1/chart/account/revenue | Dashboard chart with revenue account balance information.
*ChartsApi* | [**get_chart_category_overview**](docs/ChartsApi.md#get_chart_category_overview) | **GET** /api/v1/chart/category/overview | Dashboard chart with an overview of the users categories.
*ConfigurationApi* | [**get_configuration**](docs/ConfigurationApi.md#get_configuration) | **GET** /api/v1/configuration | Get Firefly III system configuration.
*ConfigurationApi* | [**set_configuration**](docs/ConfigurationApi.md#set_configuration) | **POST** /api/v1/configuration/{name} | Update configuration
*CurrenciesApi* | [**default_currency**](docs/CurrenciesApi.md#default_currency) | **POST** /api/v1/currencies/{code}/default | Make currency default currency.
*CurrenciesApi* | [**delete_currency**](docs/CurrenciesApi.md#delete_currency) | **DELETE** /api/v1/currencies/{code} | Delete a currency.
*CurrenciesApi* | [**disable_currency**](docs/CurrenciesApi.md#disable_currency) | **POST** /api/v1/currencies/{code}/disable | Disable a currency.
*CurrenciesApi* | [**enable_currency**](docs/CurrenciesApi.md#enable_currency) | **POST** /api/v1/currencies/{code}/enable | Enable a single currency.
*CurrenciesApi* | [**get_currency**](docs/CurrenciesApi.md#get_currency) | **GET** /api/v1/currencies/{code} | Get a single currency.
*CurrenciesApi* | [**list_account_by_currency**](docs/CurrenciesApi.md#list_account_by_currency) | **GET** /api/v1/currencies/{code}/accounts | List all accounts with this currency.
*CurrenciesApi* | [**list_available_budget_by_currency**](docs/CurrenciesApi.md#list_available_budget_by_currency) | **GET** /api/v1/currencies/{code}/available_budgets | List all available budgets with this currency.
*CurrenciesApi* | [**list_bill_by_currency**](docs/CurrenciesApi.md#list_bill_by_currency) | **GET** /api/v1/currencies/{code}/bills | List all bills with this currency.
*CurrenciesApi* | [**list_budget_limit_by_currency**](docs/CurrenciesApi.md#list_budget_limit_by_currency) | **GET** /api/v1/currencies/{code}/budget_limits | List all budget limits with this currency
*CurrenciesApi* | [**list_currency**](docs/CurrenciesApi.md#list_currency) | **GET** /api/v1/currencies | List all currencies.
*CurrenciesApi* | [**list_exchange_rate_by_currency**](docs/CurrenciesApi.md#list_exchange_rate_by_currency) | **GET** /api/v1/currencies/{code}/cer | List all known exchange rates with (from or to) this currency.
*CurrenciesApi* | [**list_recurrence_by_currency**](docs/CurrenciesApi.md#list_recurrence_by_currency) | **GET** /api/v1/currencies/{code}/recurrences | List all recurring transactions with this currency.
*CurrenciesApi* | [**list_rule_by_currency**](docs/CurrenciesApi.md#list_rule_by_currency) | **GET** /api/v1/currencies/{code}/rules | List all rules with this currency.
*CurrenciesApi* | [**list_transaction_by_currency**](docs/CurrenciesApi.md#list_transaction_by_currency) | **GET** /api/v1/currencies/{code}/transactions | List all transactions with this currency.
*CurrenciesApi* | [**store_currency**](docs/CurrenciesApi.md#store_currency) | **POST** /api/v1/currencies | Store a new currency
*CurrenciesApi* | [**update_currency**](docs/CurrenciesApi.md#update_currency) | **PUT** /api/v1/currencies/{code} | Update existing currency.
*CurrencyExchangeRatesApi* | [**get_exchange_rate**](docs/CurrencyExchangeRatesApi.md#get_exchange_rate) | **GET** /api/v1/cer | Get an exchange rate.
*ImportApi* | [**get_import**](docs/ImportApi.md#get_import) | **GET** /api/v1/import/{key} | Show info on a single import
*ImportApi* | [**list_import**](docs/ImportApi.md#list_import) | **GET** /api/v1/import/list | List al imports
*ImportApi* | [**list_transaction_by_import**](docs/ImportApi.md#list_transaction_by_import) | **GET** /api/v1/import/{key}/transactions | List all transactions related to the import job. The correlation is made through the tag.
*LinksApi* | [**delete_link_type**](docs/LinksApi.md#delete_link_type) | **DELETE** /api/v1/link_types/{id} | Permanently delete link type.
*LinksApi* | [**delete_transaction_link**](docs/LinksApi.md#delete_transaction_link) | **DELETE** /api/v1/transaction_links/{id} | Permanently delete link between transactions.
*LinksApi* | [**get_link_type**](docs/LinksApi.md#get_link_type) | **GET** /api/v1/link_types/{id} | Get single a link type.
*LinksApi* | [**get_transaction_link**](docs/LinksApi.md#get_transaction_link) | **GET** /api/v1/transaction_links/{id} | Get a single link.
*LinksApi* | [**list_link_type**](docs/LinksApi.md#list_link_type) | **GET** /api/v1/link_types | List all types of links.
*LinksApi* | [**list_transaction_by_link_type**](docs/LinksApi.md#list_transaction_by_link_type) | **GET** /api/v1/link_types/{id}/transactions | List all transactions under this link type.
*LinksApi* | [**list_transaction_link**](docs/LinksApi.md#list_transaction_link) | **GET** /api/v1/transaction_links | List all transaction links.
*LinksApi* | [**store_link_type**](docs/LinksApi.md#store_link_type) | **POST** /api/v1/link_types | Create a new link type
*LinksApi* | [**store_transaction_link**](docs/LinksApi.md#store_transaction_link) | **POST** /api/v1/transaction_links | Create a new link between transactions
*LinksApi* | [**update_link_type**](docs/LinksApi.md#update_link_type) | **PUT** /api/v1/link_types/{id} | Update existing link type.
*LinksApi* | [**update_transaction_link**](docs/LinksApi.md#update_transaction_link) | **PUT** /api/v1/transaction_links/{id} | Update an existing link between transactions.
*PiggyBanksApi* | [**delete_piggy_bank**](docs/PiggyBanksApi.md#delete_piggy_bank) | **DELETE** /api/v1/piggy_banks/{id} | Delete a piggy bank.
*PiggyBanksApi* | [**get_piggy_bank**](docs/PiggyBanksApi.md#get_piggy_bank) | **GET** /api/v1/piggy_banks/{id} | Get a single piggy bank.
*PiggyBanksApi* | [**list_event_by_piggy_bank**](docs/PiggyBanksApi.md#list_event_by_piggy_bank) | **GET** /api/v1/piggy_banks/{id}/events | List all events linked to a piggy bank.
*PiggyBanksApi* | [**list_piggy_bank**](docs/PiggyBanksApi.md#list_piggy_bank) | **GET** /api/v1/piggy_banks | List all piggy banks.
*PiggyBanksApi* | [**store_piggy_bank**](docs/PiggyBanksApi.md#store_piggy_bank) | **POST** /api/v1/piggy_banks | Store a new piggy bank
*PiggyBanksApi* | [**update_piggy_bank**](docs/PiggyBanksApi.md#update_piggy_bank) | **PUT** /api/v1/piggy_banks/{id} | Update existing piggy bank.
*PreferencesApi* | [**get_preference**](docs/PreferencesApi.md#get_preference) | **GET** /api/v1/preferences/{name} | Return a single preference.
*PreferencesApi* | [**list_preference**](docs/PreferencesApi.md#list_preference) | **GET** /api/v1/preferences | List all users preferences.
*PreferencesApi* | [**update_preference**](docs/PreferencesApi.md#update_preference) | **PUT** /api/v1/preferences/{name} | Update preference
*RecurrencesApi* | [**delete_recurrence**](docs/RecurrencesApi.md#delete_recurrence) | **DELETE** /api/v1/recurrences/{id} | Delete a recurring transaction.
*RecurrencesApi* | [**get_recurrence**](docs/RecurrencesApi.md#get_recurrence) | **GET** /api/v1/recurrences/{id} | Get a single recurring transaction.
*RecurrencesApi* | [**list_recurrence**](docs/RecurrencesApi.md#list_recurrence) | **GET** /api/v1/recurrences | List all recurring transactions.
*RecurrencesApi* | [**list_transaction_by_recurrence**](docs/RecurrencesApi.md#list_transaction_by_recurrence) | **GET** /api/v1/recurrences/{id}/transactions | List all transactions created by a recurring transaction.
*RecurrencesApi* | [**store_recurrence**](docs/RecurrencesApi.md#store_recurrence) | **POST** /api/v1/recurrences | Store a new recurring transaction
*RecurrencesApi* | [**trigger_recurrence**](docs/RecurrencesApi.md#trigger_recurrence) | **POST** /api/v1/recurrences/trigger | Trigger the creation of recurring transactions (like a cron job).
*RecurrencesApi* | [**update_recurrence**](docs/RecurrencesApi.md#update_recurrence) | **PUT** /api/v1/recurrences/{id} | Update existing recurring transaction.
*RuleGroupsApi* | [**delete_rule_group**](docs/RuleGroupsApi.md#delete_rule_group) | **DELETE** /api/v1/rule_groups/{id} | Delete a rule group.
*RuleGroupsApi* | [**fire_rule_group**](docs/RuleGroupsApi.md#fire_rule_group) | **POST** /api/v1/rule_groups/{id}/trigger | Fire the rule group on your transactions.
*RuleGroupsApi* | [**get_rule_group**](docs/RuleGroupsApi.md#get_rule_group) | **GET** /api/v1/rule_groups/{id} | Get a single rule group.
*RuleGroupsApi* | [**list_rule_by_group**](docs/RuleGroupsApi.md#list_rule_by_group) | **GET** /api/v1/rule_groups/{id}/rules | List rules in this rule group.
*RuleGroupsApi* | [**list_rule_group**](docs/RuleGroupsApi.md#list_rule_group) | **GET** /api/v1/rule_groups | List all rule groups.
*RuleGroupsApi* | [**store_rule_group**](docs/RuleGroupsApi.md#store_rule_group) | **POST** /api/v1/rule_groups | Store a new rule group.
*RuleGroupsApi* | [**test_rule_group**](docs/RuleGroupsApi.md#test_rule_group) | **GET** /api/v1/rule_groups/{id}/test | Test which transactions would be hit by the rule group. No changes will be made.
*RuleGroupsApi* | [**update_rule_group**](docs/RuleGroupsApi.md#update_rule_group) | **PUT** /api/v1/rule_groups/{id} | Update existing rule group.
*RulesApi* | [**delete_rule**](docs/RulesApi.md#delete_rule) | **DELETE** /api/v1/rules/{id} | Delete an rule.
*RulesApi* | [**fire_rule**](docs/RulesApi.md#fire_rule) | **POST** /api/v1/rules/{id}/trigger | Fire the rule on your transactions.
*RulesApi* | [**get_rule**](docs/RulesApi.md#get_rule) | **GET** /api/v1/rules/{id} | Get a single rule.
*RulesApi* | [**list_rule**](docs/RulesApi.md#list_rule) | **GET** /api/v1/rules | List all rules.
*RulesApi* | [**store_rule**](docs/RulesApi.md#store_rule) | **POST** /api/v1/rules | Store a new rule
*RulesApi* | [**test_rule**](docs/RulesApi.md#test_rule) | **GET** /api/v1/rules/{id}/test | Test which transactions would be hit by the rule. No changes will be made.
*RulesApi* | [**update_rule**](docs/RulesApi.md#update_rule) | **PUT** /api/v1/rules/{id} | Update existing rule.
*SummaryApi* | [**get_basic_summary**](docs/SummaryApi.md#get_basic_summary) | **GET** /api/v1/summary/basic | Returns basic sums of the users data.
*TagsApi* | [**delete_tag**](docs/TagsApi.md#delete_tag) | **DELETE** /api/v1/tags/{tag_id} | Delete an tag.
*TagsApi* | [**get_tag**](docs/TagsApi.md#get_tag) | **GET** /api/v1/tags/{tag_id} | Get a single tag.
*TagsApi* | [**get_tag_cloud**](docs/TagsApi.md#get_tag_cloud) | **GET** /api/v1/tag-cloud | Returns a basic tag cloud.
*TagsApi* | [**list_tag**](docs/TagsApi.md#list_tag) | **GET** /api/v1/tags | List all tags.
*TagsApi* | [**list_transaction_by_tag**](docs/TagsApi.md#list_transaction_by_tag) | **GET** /api/v1/tags/{tag_id}/transactions | List all transactions with this tag.
*TagsApi* | [**store_tag**](docs/TagsApi.md#store_tag) | **POST** /api/v1/tags | Store a new tag
*TagsApi* | [**update_tag**](docs/TagsApi.md#update_tag) | **PUT** /api/v1/tags/{tag_id} | Update existing tag.
*TransactionsApi* | [**delete_transaction**](docs/TransactionsApi.md#delete_transaction) | **DELETE** /api/v1/transactions/{id} | Delete a transaction.
*TransactionsApi* | [**get_transaction**](docs/TransactionsApi.md#get_transaction) | **GET** /api/v1/transactions/{id} | Get a single transaction.
*TransactionsApi* | [**get_transaction_by_journal**](docs/TransactionsApi.md#get_transaction_by_journal) | **GET** /api/v1/transaction-journals/{id} | Get a single transaction, based on one of the underlying transaction journals.
*TransactionsApi* | [**list_attachment_by_transaction**](docs/TransactionsApi.md#list_attachment_by_transaction) | **GET** /api/v1/transactions/{id}/attachments | Lists all attachments.
*TransactionsApi* | [**list_event_by_transaction**](docs/TransactionsApi.md#list_event_by_transaction) | **GET** /api/v1/transactions/{id}/piggy_bank_events | Lists all piggy bank events.
*TransactionsApi* | [**list_transaction**](docs/TransactionsApi.md#list_transaction) | **GET** /api/v1/transactions | List all the user's transactions.
*TransactionsApi* | [**store_transaction**](docs/TransactionsApi.md#store_transaction) | **POST** /api/v1/transactions | Store a new transaction
*TransactionsApi* | [**update_transaction**](docs/TransactionsApi.md#update_transaction) | **PUT** /api/v1/transactions/{id} | Update existing transaction.
*UsersApi* | [**delete_user**](docs/UsersApi.md#delete_user) | **DELETE** /api/v1/users/{id} | Delete a user.
*UsersApi* | [**get_user**](docs/UsersApi.md#get_user) | **GET** /api/v1/users/{id} | Get a single user.
*UsersApi* | [**list_user**](docs/UsersApi.md#list_user) | **GET** /api/v1/users | List all users.
*UsersApi* | [**store_user**](docs/UsersApi.md#store_user) | **POST** /api/v1/users | Store a new user
*UsersApi* | [**update_user**](docs/UsersApi.md#update_user) | **PUT** /api/v1/users/{id} | Update an existing user's information.


## Documentation For Models

 - [Account](docs/Account.md)
 - [AccountArray](docs/AccountArray.md)
 - [AccountRead](docs/AccountRead.md)
 - [AccountSingle](docs/AccountSingle.md)
 - [Attachment](docs/Attachment.md)
 - [AttachmentArray](docs/AttachmentArray.md)
 - [AttachmentRead](docs/AttachmentRead.md)
 - [AttachmentSingle](docs/AttachmentSingle.md)
 - [AvailableBudget](docs/AvailableBudget.md)
 - [AvailableBudgetArray](docs/AvailableBudgetArray.md)
 - [AvailableBudgetRead](docs/AvailableBudgetRead.md)
 - [AvailableBudgetSingle](docs/AvailableBudgetSingle.md)
 - [BasicSummaryEntry](docs/BasicSummaryEntry.md)
 - [Bill](docs/Bill.md)
 - [BillArray](docs/BillArray.md)
 - [BillPaidDates](docs/BillPaidDates.md)
 - [BillRead](docs/BillRead.md)
 - [BillSingle](docs/BillSingle.md)
 - [Budget](docs/Budget.md)
 - [BudgetArray](docs/BudgetArray.md)
 - [BudgetLimit](docs/BudgetLimit.md)
 - [BudgetLimitArray](docs/BudgetLimitArray.md)
 - [BudgetLimitRead](docs/BudgetLimitRead.md)
 - [BudgetLimitSingle](docs/BudgetLimitSingle.md)
 - [BudgetRead](docs/BudgetRead.md)
 - [BudgetSingle](docs/BudgetSingle.md)
 - [BudgetSpent](docs/BudgetSpent.md)
 - [Category](docs/Category.md)
 - [CategoryArray](docs/CategoryArray.md)
 - [CategoryEarned](docs/CategoryEarned.md)
 - [CategoryRead](docs/CategoryRead.md)
 - [CategorySingle](docs/CategorySingle.md)
 - [CategorySpent](docs/CategorySpent.md)
 - [ChartDataPoint](docs/ChartDataPoint.md)
 - [ChartDataSet](docs/ChartDataSet.md)
 - [Configuration](docs/Configuration.md)
 - [ConfigurationData](docs/ConfigurationData.md)
 - [ConfigurationUpdate](docs/ConfigurationUpdate.md)
 - [Currency](docs/Currency.md)
 - [CurrencyArray](docs/CurrencyArray.md)
 - [CurrencyRead](docs/CurrencyRead.md)
 - [CurrencySingle](docs/CurrencySingle.md)
 - [ExchangeRate](docs/ExchangeRate.md)
 - [ExchangeRateArray](docs/ExchangeRateArray.md)
 - [ExchangeRateAttributes](docs/ExchangeRateAttributes.md)
 - [ImportJob](docs/ImportJob.md)
 - [ImportJobArray](docs/ImportJobArray.md)
 - [ImportJobAttributes](docs/ImportJobAttributes.md)
 - [ImportJobSingle](docs/ImportJobSingle.md)
 - [LinkType](docs/LinkType.md)
 - [LinkTypeArray](docs/LinkTypeArray.md)
 - [LinkTypeRead](docs/LinkTypeRead.md)
 - [LinkTypeSingle](docs/LinkTypeSingle.md)
 - [Meta](docs/Meta.md)
 - [MetaPagination](docs/MetaPagination.md)
 - [ObjectLink](docs/ObjectLink.md)
 - [ObjectLink0](docs/ObjectLink0.md)
 - [PageLink](docs/PageLink.md)
 - [PiggyBank](docs/PiggyBank.md)
 - [PiggyBankArray](docs/PiggyBankArray.md)
 - [PiggyBankEvent](docs/PiggyBankEvent.md)
 - [PiggyBankEventArray](docs/PiggyBankEventArray.md)
 - [PiggyBankEventAttributes](docs/PiggyBankEventAttributes.md)
 - [PiggyBankRead](docs/PiggyBankRead.md)
 - [PiggyBankSingle](docs/PiggyBankSingle.md)
 - [Preference](docs/Preference.md)
 - [PreferenceArray](docs/PreferenceArray.md)
 - [PreferenceRead](docs/PreferenceRead.md)
 - [PreferenceSingle](docs/PreferenceSingle.md)
 - [Recurrence](docs/Recurrence.md)
 - [RecurrenceArray](docs/RecurrenceArray.md)
 - [RecurrenceRead](docs/RecurrenceRead.md)
 - [RecurrenceRepetition](docs/RecurrenceRepetition.md)
 - [RecurrenceSingle](docs/RecurrenceSingle.md)
 - [RecurrenceTransaction](docs/RecurrenceTransaction.md)
 - [Rule](docs/Rule.md)
 - [RuleAction](docs/RuleAction.md)
 - [RuleArray](docs/RuleArray.md)
 - [RuleGroup](docs/RuleGroup.md)
 - [RuleGroupArray](docs/RuleGroupArray.md)
 - [RuleGroupRead](docs/RuleGroupRead.md)
 - [RuleGroupSingle](docs/RuleGroupSingle.md)
 - [RuleRead](docs/RuleRead.md)
 - [RuleSingle](docs/RuleSingle.md)
 - [RuleTrigger](docs/RuleTrigger.md)
 - [SystemInfo](docs/SystemInfo.md)
 - [SystemInfoData](docs/SystemInfoData.md)
 - [Tag](docs/Tag.md)
 - [TagArray](docs/TagArray.md)
 - [TagCloud](docs/TagCloud.md)
 - [TagCloudTag](docs/TagCloudTag.md)
 - [TagRead](docs/TagRead.md)
 - [TagSingle](docs/TagSingle.md)
 - [Transaction](docs/Transaction.md)
 - [TransactionArray](docs/TransactionArray.md)
 - [TransactionLink](docs/TransactionLink.md)
 - [TransactionLinkArray](docs/TransactionLinkArray.md)
 - [TransactionLinkRead](docs/TransactionLinkRead.md)
 - [TransactionLinkSingle](docs/TransactionLinkSingle.md)
 - [TransactionRead](docs/TransactionRead.md)
 - [TransactionSingle](docs/TransactionSingle.md)
 - [TransactionSplit](docs/TransactionSplit.md)
 - [User](docs/User.md)
 - [UserArray](docs/UserArray.md)
 - [UserRead](docs/UserRead.md)
 - [UserSingle](docs/UserSingle.md)
 - [ValidationError](docs/ValidationError.md)
 - [ValidationErrorErrors](docs/ValidationErrorErrors.md)


To get access to the crate's generated documentation, use:

```
cargo doc --open
```

## Author

thegrumpydictator@gmail.com
