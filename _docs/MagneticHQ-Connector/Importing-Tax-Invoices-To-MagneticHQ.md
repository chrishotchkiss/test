---
slug: importing-tax-invoices-to-magnetichq
redirect_from: "/article/importing-tax-invoices-to-magnetichq"
title: Importing Tax Invoices to Magnetic HQ
---
This task will import tax invoices that are supplied in an XML format.

## Settings
### Connection
_Required_  
The MagneticHQ connection to use. See the [Connecting to MagentoHQ](connecting-to-magnetichq) if you require more information on how to create/manage connections.

### Fail File
_Required_  
The name of a file for "failed" imports to be sent to.

### Input File
_Required_  
The source file that you want to import in Zynk XML format.

### Success File
_Required_  
The name of a file for "successful" imports to be sent to. 

### Zynk Settings
See [Common Task Settings](common-task-settings).

## Examples
A sample input file is shown below.
```xml
<?xml version="1.0" encoding="utf-8"?>
<MagneticHQData xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <TaxInvoices>
    <TaxInvoice>
      <Account>
        <Id>54067397</Id>
        <Version>4</Version>
        <Name>New Filming</Name>
        <RefCode>0001</RefCode>
        <Status>DRAFT</Status>
        <Description />
        <OrderCode />
        <PaymentTerms>30 Days</PaymentTerms>
        <Billed>100.0</Billed>
        <Tax>14.0</Tax>
        <Cost>500.0</Cost>
        <CurrencyCost>500.0</CurrencyCost>
        <Margin>500.0</Margin>
        <CurrencyMargin>500.0</CurrencyMargin>
        <TotalCost>570.0</TotalCost>
        <CurrencyTotalCost>570.0</CurrencyTotalCost>
        <CreatedDate>1447740000000</CreatedDate>
        <IssuedDate>0</IssuedDate>
        <Company>
          <Id>53126881</Id>
          <Version>4</Version>
          <Name>Zynk Ltd</Name>
          <ContactPerson>Nathan Hopkins</ContactPerson>
          <BillingName />
          <ContactNumber />
          <EmailAddress>Nathan@Zynk.com</EmailAddress>
          <PhysicalAddress />
          <PostalAddress />
          <Website />
          <MailDomain>Zynk.com</MailDomain>
          <Description />
          <CreatedDate>1446815017313</CreatedDate>
          <OtherInfo></OtherInfo>
          <ExternalReference />
          <Tag>lead</Tag>
          <TaxNumber />
          <KeyPerson>
            <Id>53126884</Id>
            <Version>2</Version>
            <Title>Mr</Title>
            <FirstName>Nathan</FirstName>
            <LastName>Hopkins</LastName>
            <FullName>Nathan Hopkins</FullName>
            <LandNumber />
            <CellNumber />
            <FaxNumber />
            <Email>Nathan@Zynk.com</Email>
            <PhysicalAddress />
            <PostalAddress />
            <Position>KTP Associate</Position>
            <OtherInfo>Manufacture of lifting and handling equipment</OtherInfo>
            <ExternalReference />
            <Tag />
            <CreatedDate>1446815017357</CreatedDate>
            <Owner>
              <Id>53090727</Id>
              <Version>200</Version>
              <Title>Studio Manager</Title>
              <FirstName>Oliver</FirstName>
              <LastName>Jeffery</LastName>
              <FullName>Oliver Jeffery</FullName>
              <Email>magnetic@email.co.uk</Email>
              <ContactNumber>07123456789</ContactNumber>
              <Description />
              <UserName>magnetic@email.co.uk</UserName>
              <RoleType>ADMIN</RoleType>
              <UserManager>true</UserManager>
              <Skin>bing</Skin>
              <Accounts>true</Accounts>
              <Grouping>Design</Grouping>
              <CreatedDate>1446813531845</CreatedDate>
              <LastAccessedDate>1503412276262</LastAccessedDate>
              <LoginAttempts>0</LoginAttempts>
              <TimeTrackingUser>false</TimeTrackingUser>
              <NoWorkDone>1446731581084</NoWorkDone>
              <PageSize>40</PageSize>
              <Status>ACTIVATED</Status>
              <AccountsAdministrator>true</AccountsAdministrator>
              <AddGroupings>true</AddGroupings>
              <NotifyMethod>EMAIL</NotifyMethod>
              <HrManager>true</HrManager>
              <TimeZone>36,GMT+02:00</TimeZone>
              <ReceiveDailyNotification>false</ReceiveDailyNotification>
              <ReceiveRealtimeNotifications>true</ReceiveRealtimeNotifications>
              <HideDetails>false</HideDetails>
              <TaskView>LIST</TaskView>
              <GroupingSignedView>STATUSLANE</GroupingSignedView>
              <GroupingUnsignedView>LIST</GroupingUnsignedView>
              <Type>SALES</Type>
              <RewardStatus>NONE</RewardStatus>
              <AnnualLeave>26</AnnualLeave>
              <SickLeave>0</SickLeave>
              <CompassionateLeave>0</CompassionateLeave>
              <OtherLeave>0</OtherLeave>
              <ReceiveHrEmails>true</ReceiveHrEmails>
              <HourCapacityPerDay>8.0</HourCapacityPerDay>
              <EmployeeCost>0.0</EmployeeCost>
              <CostEstimatePermission>WRITE_APPROVE</CostEstimatePermission>
              <PurchaseOrderPermission>WRITE</PurchaseOrderPermission>
              <TaxInvoicePermission>WRITE</TaxInvoicePermission>
              <SupplierInvoicePermission>WRITE</SupplierInvoicePermission>
              <ExpensePermission>NONE</ExpensePermission>
              <Active>true</Active>
              <FirstLastInitial>Oliver J</FirstLastInitial>
            </Owner>
            <Global>true</Global>
            <CustomFields />
          </KeyPerson>
          <Owner>
            <Id>53090727</Id>
            <Version>200</Version>
            <Title>Studio Manager</Title>
            <FirstName>Oliver</FirstName>
            <LastName>Jeffery</LastName>
            <FullName>Oliver Jeffery</FullName>
            <Email>magnetic@email.co.uk</Email>
            <ContactNumber>07123456789</ContactNumber>
            <Description />
            <UserName>magnetic@email.co.uk</UserName>
            <RoleType>ADMIN</RoleType>
            <UserManager>true</UserManager>
            <Skin>bing</Skin>
            <Accounts>true</Accounts>
            <Grouping>Design</Grouping>
            <CreatedDate>1446813531845</CreatedDate>
            <LastAccessedDate>1503412276262</LastAccessedDate>
            <LoginAttempts>0</LoginAttempts>
            <TimeTrackingUser>false</TimeTrackingUser>
            <NoWorkDone>1446731581084</NoWorkDone>
            <PageSize>40</PageSize>
            <Status>ACTIVATED</Status>
            <AccountsAdministrator>true</AccountsAdministrator>
            <AddGroupings>true</AddGroupings>
            <NotifyMethod>EMAIL</NotifyMethod>
            <HrManager>true</HrManager>
            <TimeZone>36,GMT+02:00</TimeZone>
            <ReceiveDailyNotification>false</ReceiveDailyNotification>
            <ReceiveRealtimeNotifications>true</ReceiveRealtimeNotifications>
            <HideDetails>false</HideDetails>
            <TaskView>LIST</TaskView>
            <GroupingSignedView>STATUSLANE</GroupingSignedView>
            <GroupingUnsignedView>LIST</GroupingUnsignedView>
            <Type>SALES</Type>
            <RewardStatus>NONE</RewardStatus>
            <AnnualLeave>26</AnnualLeave>
            <SickLeave>0</SickLeave>
            <CompassionateLeave>0</CompassionateLeave>
            <OtherLeave>0</OtherLeave>
            <ReceiveHrEmails>true</ReceiveHrEmails>
            <HourCapacityPerDay>8.0</HourCapacityPerDay>
            <EmployeeCost>0.0</EmployeeCost>
            <CostEstimatePermission>WRITE_APPROVE</CostEstimatePermission>
            <PurchaseOrderPermission>WRITE</PurchaseOrderPermission>
            <TaxInvoicePermission>WRITE</TaxInvoicePermission>
            <SupplierInvoicePermission>WRITE</SupplierInvoicePermission>
            <ExpensePermission>NONE</ExpensePermission>
            <Active>true</Active>
            <FirstLastInitial>Oliver J</FirstLastInitial>
          </Owner>
          <Global>true</Global>
          <ApprovedAccountsCustomer>false</ApprovedAccountsCustomer>
          <ApprovedAccountsSupplier>false</ApprovedAccountsSupplier>
          <LastActivityDate>0</LastActivityDate>
          <CustomFields>
            <item>
              <key>53134950</key>
              <value />
            </item>
            <item>
              <key>53130868</key>
              <value>1448316000000</value>
            </item>
            <item>
              <key>53179986</key>
              <value>Manufacture of lifting and handling equipment</value>
            </item>
            <item>
              <key>53130884</key>
              <value>Test</value>
            </item>
            <item>
              <key>53164750</key>
              <value>Oliver Jeffery</value>
            </item>
            <item>
              <key>53164698</key>
              <value>12</value>
            </item>
          </CustomFields>
          <ModifiedDate>1446815017313</ModifiedDate>
        </Company>
        <DeliveryAddress />
        <Contact>
          <Id>53126884</Id>
          <Version>2</Version>
          <Title>Mr</Title>
          <FirstName>Nathan</FirstName>
          <LastName>Hopkins</LastName>
          <FullName>Nathan Hopkins</FullName>
          <LandNumber />
          <CellNumber />
          <FaxNumber />
          <Email>Nathan@Zynk.com</Email>
          <PhysicalAddress />
          <PostalAddress />
          <Position>KTP Associate</Position>
          <OtherInfo>Manufacture of lifting and handling equipment</OtherInfo>
          <ExternalReference />
          <Tag />
          <CreatedDate>1446815017357</CreatedDate>
          <Owner>
            <Id>53090727</Id>
            <Version>200</Version>
            <Title>Studio Manager</Title>
            <FirstName>Oliver</FirstName>
            <LastName>Jeffery</LastName>
            <FullName>Oliver Jeffery</FullName>
            <Email>magnetic@email.co.uk</Email>
            <ContactNumber>07123456789</ContactNumber>
            <Description />
            <UserName>magnetic@email.co.uk</UserName>
            <RoleType>ADMIN</RoleType>
            <UserManager>true</UserManager>
            <Skin>bing</Skin>
            <Accounts>true</Accounts>
            <Grouping>Design</Grouping>
            <CreatedDate>1446813531845</CreatedDate>
            <LastAccessedDate>1503412276262</LastAccessedDate>
            <LoginAttempts>0</LoginAttempts>
            <TimeTrackingUser>false</TimeTrackingUser>
            <NoWorkDone>1446731581084</NoWorkDone>
            <PageSize>40</PageSize>
            <Status>ACTIVATED</Status>
            <AccountsAdministrator>true</AccountsAdministrator>
            <AddGroupings>true</AddGroupings>
            <NotifyMethod>EMAIL</NotifyMethod>
            <HrManager>true</HrManager>
            <TimeZone>36,GMT+02:00</TimeZone>
            <ReceiveDailyNotification>false</ReceiveDailyNotification>
            <ReceiveRealtimeNotifications>true</ReceiveRealtimeNotifications>
            <HideDetails>false</HideDetails>
            <TaskView>LIST</TaskView>
            <GroupingSignedView>STATUSLANE</GroupingSignedView>
            <GroupingUnsignedView>LIST</GroupingUnsignedView>
            <Type>SALES</Type>
            <RewardStatus>NONE</RewardStatus>
            <AnnualLeave>26</AnnualLeave>
            <SickLeave>0</SickLeave>
            <CompassionateLeave>0</CompassionateLeave>
            <OtherLeave>0</OtherLeave>
            <ReceiveHrEmails>true</ReceiveHrEmails>
            <HourCapacityPerDay>8.0</HourCapacityPerDay>
            <EmployeeCost>0.0</EmployeeCost>
            <CostEstimatePermission>WRITE_APPROVE</CostEstimatePermission>
            <PurchaseOrderPermission>WRITE</PurchaseOrderPermission>
            <TaxInvoicePermission>WRITE</TaxInvoicePermission>
            <SupplierInvoicePermission>WRITE</SupplierInvoicePermission>
            <ExpensePermission>NONE</ExpensePermission>
            <Active>true</Active>
            <FirstLastInitial>Oliver J</FirstLastInitial>
          </Owner>
          <Global>true</Global>
          <CustomFields />
        </Contact>
        <Grouping>
          <Id>53130779</Id>
          <Version>10</Version>
          <Code>0003</Code>
          <Name>Zynk - Document Mailer</Name>
          <Extra></Extra>
          <Access>PUBLIC</Access>
          <CreatedDate>1446816296512</CreatedDate>
          <CustomFields>
            <item>
              <key>60050127</key>
              <value>Branding</value>
            </item>
            <item>
              <key>60050128</key>
              <value>1448316000000</value>
            </item>
            <item>
              <key>60050129</key>
              <value>Website</value>
            </item>
          </CustomFields>
          <ModifiedDate>1447764659068</ModifiedDate>
          <SignedDate>1447764659098</SignedDate>
          <StartDate>1447764659098</StartDate>
          <EndDate>1455713459300</EndDate>
          <ExternalReference>(m#00030)</ExternalReference>
          <Signed>true</Signed>
          <Status />
          <Amount>10000.0</Amount>
          <MonthlyAmount>1000.0</MonthlyAmount>
          <PercentageComplete>0</PercentageComplete>
          <Complete>false</Complete>
          <Archive>false</Archive>
          <Tag>Mailer</Tag>
          <TaskStatuses />
          <ContactCompany>
            <Id>53126881</Id>
            <Version>4</Version>
            <Name>Zynk Ltd</Name>
            <ContactPerson>Nathan Hopkins</ContactPerson>
            <BillingName />
            <ContactNumber />
            <EmailAddress>Nathan@Zynk.com</EmailAddress>
            <PhysicalAddress />
            <PostalAddress />
            <Website />
            <MailDomain>Zynk.com</MailDomain>
            <Description />
            <CreatedDate>1446815017313</CreatedDate>
            <OtherInfo>Manufacture of lifting and handling equipment</OtherInfo>
            <ExternalReference />
            <Tag>lead</Tag>
            <TaxNumber />
            <KeyPerson>
              <Id>53126884</Id>
              <Version>2</Version>
              <Title>Mr</Title>
              <FirstName>Nathan</FirstName>
              <LastName>Hopkins</LastName>
              <FullName>Nathan Hopkins</FullName>
              <LandNumber />
              <CellNumber />
              <FaxNumber />
              <Email>Nathan@Zynk.com</Email>
              <PhysicalAddress />
              <PostalAddress />
              <Position>KTP Associate</Position>
              <OtherInfo>Manufacture of lifting and handling equipment</OtherInfo>
              <ExternalReference />
              <Tag />
              <CreatedDate>1446815017357</CreatedDate>
              <Owner>
                <Id>53090727</Id>
                <Version>200</Version>
                <Title>Studio Manager</Title>
                <FirstName>Oliver</FirstName>
                <LastName>Jeffery</LastName>
                <FullName>Oliver Jeffery</FullName>
                <Email>magnetic@email.co.uk</Email>
                <ContactNumber>07123456789</ContactNumber>
                <Description />
                <UserName>magnetic@email.co.uk</UserName>
                <RoleType>ADMIN</RoleType>
                <UserManager>true</UserManager>
                <Skin>bing</Skin>
                <Accounts>true</Accounts>
                <Grouping>Design</Grouping>
                <CreatedDate>1446813531845</CreatedDate>
                <LastAccessedDate>1503412276262</LastAccessedDate>
                <LoginAttempts>0</LoginAttempts>
                <TimeTrackingUser>false</TimeTrackingUser>
                <NoWorkDone>1446731581084</NoWorkDone>
                <PageSize>40</PageSize>
                <Status>ACTIVATED</Status>
                <AccountsAdministrator>true</AccountsAdministrator>
                <AddGroupings>true</AddGroupings>
                <NotifyMethod>EMAIL</NotifyMethod>
                <HrManager>true</HrManager>
                <TimeZone>36,GMT+02:00</TimeZone>
                <ReceiveDailyNotification>false</ReceiveDailyNotification>
                <ReceiveRealtimeNotifications>true</ReceiveRealtimeNotifications>
                <HideDetails>false</HideDetails>
                <TaskView>LIST</TaskView>
                <GroupingSignedView>STATUSLANE</GroupingSignedView>
                <GroupingUnsignedView>LIST</GroupingUnsignedView>
                <Type>SALES</Type>
                <RewardStatus>NONE</RewardStatus>
                <AnnualLeave>26</AnnualLeave>
                <SickLeave>0</SickLeave>
                <CompassionateLeave>0</CompassionateLeave>
                <OtherLeave>0</OtherLeave>
                <ReceiveHrEmails>true</ReceiveHrEmails>
                <HourCapacityPerDay>8.0</HourCapacityPerDay>
                <EmployeeCost>0.0</EmployeeCost>
                <CostEstimatePermission>WRITE_APPROVE</CostEstimatePermission>
                <PurchaseOrderPermission>WRITE</PurchaseOrderPermission>
                <TaxInvoicePermission>WRITE</TaxInvoicePermission>
                <SupplierInvoicePermission>WRITE</SupplierInvoicePermission>
                <ExpensePermission>NONE</ExpensePermission>
                <Active>true</Active>
                <FirstLastInitial>Oliver J</FirstLastInitial>
              </Owner>
              <Global>true</Global>
              <CustomFields />
            </KeyPerson>
            <Owner>
              <Id>53090727</Id>
              <Version>200</Version>
              <Title>Studio Manager</Title>
              <FirstName>Oliver</FirstName>
              <LastName>Jeffery</LastName>
              <FullName>Oliver Jeffery</FullName>
              <Email>magnetic@email.co.uk</Email>
              <ContactNumber>07123456789</ContactNumber>
              <Description />
              <UserName>magnetic@email.co.uk</UserName>
              <RoleType>ADMIN</RoleType>
              <UserManager>true</UserManager>
              <Skin>bing</Skin>
              <Accounts>true</Accounts>
              <Grouping>Design</Grouping>
              <CreatedDate>1446813531845</CreatedDate>
              <LastAccessedDate>1503412276262</LastAccessedDate>
              <LoginAttempts>0</LoginAttempts>
              <TimeTrackingUser>false</TimeTrackingUser>
              <NoWorkDone>1446731581084</NoWorkDone>
              <PageSize>40</PageSize>
              <Status>ACTIVATED</Status>
              <AccountsAdministrator>true</AccountsAdministrator>
              <AddGroupings>true</AddGroupings>
              <NotifyMethod>EMAIL</NotifyMethod>
              <HrManager>true</HrManager>
              <TimeZone>36,GMT+02:00</TimeZone>
              <ReceiveDailyNotification>false</ReceiveDailyNotification>
              <ReceiveRealtimeNotifications>true</ReceiveRealtimeNotifications>
              <HideDetails>false</HideDetails>
              <TaskView>LIST</TaskView>
              <GroupingSignedView>STATUSLANE</GroupingSignedView>
              <GroupingUnsignedView>LIST</GroupingUnsignedView>
              <Type>SALES</Type>
              <RewardStatus>NONE</RewardStatus>
              <AnnualLeave>26</AnnualLeave>
              <SickLeave>0</SickLeave>
              <CompassionateLeave>0</CompassionateLeave>
              <OtherLeave>0</OtherLeave>
              <ReceiveHrEmails>true</ReceiveHrEmails>
              <HourCapacityPerDay>8.0</HourCapacityPerDay>
              <EmployeeCost>0.0</EmployeeCost>
              <CostEstimatePermission>WRITE_APPROVE</CostEstimatePermission>
              <PurchaseOrderPermission>WRITE</PurchaseOrderPermission>
              <TaxInvoicePermission>WRITE</TaxInvoicePermission>
              <SupplierInvoicePermission>WRITE</SupplierInvoicePermission>
              <ExpensePermission>NONE</ExpensePermission>
              <Active>true</Active>
              <FirstLastInitial>Oliver J</FirstLastInitial>
            </Owner>
            <Global>true</Global>
            <ApprovedAccountsCustomer>false</ApprovedAccountsCustomer>
            <ApprovedAccountsSupplier>false</ApprovedAccountsSupplier>
            <LastActivityDate>0</LastActivityDate>
            <CustomFields>
              <item>
                <key>53134950</key>
                <value />
              </item>
              <item>
                <key>53130868</key>
                <value>1448316000000</value>
              </item>
              <item>
                <key>53179986</key>
                <value>Manufacture of lifting and handling equipment</value>
              </item>
              <item>
                <key>53130884</key>
                <value>Test</value>
              </item>
              <item>
                <key>53164750</key>
                <value>Oliver Jeffery</value>
              </item>
              <item>
                <key>53164698</key>
                <value>12</value>
              </item>
            </CustomFields>
            <ModifiedDate>1446815017313</ModifiedDate>
          </ContactCompany>
          <Contact>
            <Id>53126884</Id>
            <Version>2</Version>
            <Title>Mr</Title>
            <FirstName>Nathan</FirstName>
            <LastName>Hopkins</LastName>
            <FullName>Nathan Hopkins</FullName>
            <LandNumber />
            <CellNumber />
            <FaxNumber />
            <Email>Nathan@Zynk.com</Email>
            <PhysicalAddress />
            <PostalAddress />
            <Position>KTP Associate</Position>
            <OtherInfo>Manufacture of lifting and handling equipment</OtherInfo>
            <ExternalReference />
            <Tag />
            <CreatedDate>1446815017357</CreatedDate>
            <Owner>
              <Id>53090727</Id>
              <Version>200</Version>
              <Title>Studio Manager</Title>
              <FirstName>Oliver</FirstName>
              <LastName>Jeffery</LastName>
              <FullName>Oliver Jeffery</FullName>
              <Email>magnetic@email.co.uk</Email>
              <ContactNumber>07123456789</ContactNumber>
              <Description />
              <UserName>magnetic@email.co.uk</UserName>
              <RoleType>ADMIN</RoleType>
              <UserManager>true</UserManager>
              <Skin>bing</Skin>
              <Accounts>true</Accounts>
              <Grouping>Design</Grouping>
              <CreatedDate>1446813531845</CreatedDate>
              <LastAccessedDate>1503412276262</LastAccessedDate>
              <LoginAttempts>0</LoginAttempts>
              <TimeTrackingUser>false</TimeTrackingUser>
              <NoWorkDone>1446731581084</NoWorkDone>
              <PageSize>40</PageSize>
              <Status>ACTIVATED</Status>
              <AccountsAdministrator>true</AccountsAdministrator>
              <AddGroupings>true</AddGroupings>
              <NotifyMethod>EMAIL</NotifyMethod>
              <HrManager>true</HrManager>
              <TimeZone>36,GMT+02:00</TimeZone>
              <ReceiveDailyNotification>false</ReceiveDailyNotification>
              <ReceiveRealtimeNotifications>true</ReceiveRealtimeNotifications>
              <HideDetails>false</HideDetails>
              <TaskView>LIST</TaskView>
              <GroupingSignedView>STATUSLANE</GroupingSignedView>
              <GroupingUnsignedView>LIST</GroupingUnsignedView>
              <Type>SALES</Type>
              <RewardStatus>NONE</RewardStatus>
              <AnnualLeave>26</AnnualLeave>
              <SickLeave>0</SickLeave>
              <CompassionateLeave>0</CompassionateLeave>
              <OtherLeave>0</OtherLeave>
              <ReceiveHrEmails>true</ReceiveHrEmails>
              <HourCapacityPerDay>8.0</HourCapacityPerDay>
              <EmployeeCost>0.0</EmployeeCost>
              <CostEstimatePermission>WRITE_APPROVE</CostEstimatePermission>
              <PurchaseOrderPermission>WRITE</PurchaseOrderPermission>
              <TaxInvoicePermission>WRITE</TaxInvoicePermission>
              <SupplierInvoicePermission>WRITE</SupplierInvoicePermission>
              <ExpensePermission>NONE</ExpensePermission>
              <Active>true</Active>
              <FirstLastInitial>Oliver J</FirstLastInitial>
            </Owner>
            <Global>true</Global>
            <CustomFields />
          </Contact>
          <Owner>
            <Id>53090727</Id>
            <Version>200</Version>
            <Title>Studio Manager</Title>
            <FirstName>Oliver</FirstName>
            <LastName>Jeffery</LastName>
            <FullName>Oliver Jeffery</FullName>
            <Email>magnetic@email.co.uk</Email>
            <ContactNumber>07123456789</ContactNumber>
            <Description />
            <UserName>magnetic@email.co.uk</UserName>
            <RoleType>ADMIN</RoleType>
            <UserManager>true</UserManager>
            <Skin>bing</Skin>
            <Accounts>true</Accounts>
            <Grouping>Design</Grouping>
            <CreatedDate>1446813531845</CreatedDate>
            <LastAccessedDate>1503412276262</LastAccessedDate>
            <LoginAttempts>0</LoginAttempts>
            <TimeTrackingUser>false</TimeTrackingUser>
            <NoWorkDone>1446731581084</NoWorkDone>
            <PageSize>40</PageSize>
            <Status>ACTIVATED</Status>
            <AccountsAdministrator>true</AccountsAdministrator>
            <AddGroupings>true</AddGroupings>
            <NotifyMethod>EMAIL</NotifyMethod>
            <HrManager>true</HrManager>
            <TimeZone>36,GMT+02:00</TimeZone>
            <ReceiveDailyNotification>false</ReceiveDailyNotification>
            <ReceiveRealtimeNotifications>true</ReceiveRealtimeNotifications>
            <HideDetails>false</HideDetails>
            <TaskView>LIST</TaskView>
            <GroupingSignedView>STATUSLANE</GroupingSignedView>
            <GroupingUnsignedView>LIST</GroupingUnsignedView>
            <Type>SALES</Type>
            <RewardStatus>NONE</RewardStatus>
            <AnnualLeave>26</AnnualLeave>
            <SickLeave>0</SickLeave>
            <CompassionateLeave>0</CompassionateLeave>
            <OtherLeave>0</OtherLeave>
            <ReceiveHrEmails>true</ReceiveHrEmails>
            <HourCapacityPerDay>8.0</HourCapacityPerDay>
            <EmployeeCost>0.0</EmployeeCost>
            <CostEstimatePermission>WRITE_APPROVE</CostEstimatePermission>
            <PurchaseOrderPermission>WRITE</PurchaseOrderPermission>
            <TaxInvoicePermission>WRITE</TaxInvoicePermission>
            <SupplierInvoicePermission>WRITE</SupplierInvoicePermission>
            <ExpensePermission>NONE</ExpensePermission>
            <Active>true</Active>
            <FirstLastInitial>Oliver J</FirstLastInitial>
          </Owner>
          <Author>
            <Id>53090727</Id>
            <Version>200</Version>
            <Title>Studio Manager</Title>
            <FirstName>Oliver</FirstName>
            <LastName>Jeffery</LastName>
            <FullName>Oliver Jeffery</FullName>
            <Email>magnetic@email.co.uk</Email>
            <ContactNumber>07123456789</ContactNumber>
            <Description />
            <UserName>magnetic@email.co.uk</UserName>
            <RoleType>ADMIN</RoleType>
            <UserManager>true</UserManager>
            <Skin>bing</Skin>
            <Accounts>true</Accounts>
            <Grouping>Design</Grouping>
            <CreatedDate>1446813531845</CreatedDate>
            <LastAccessedDate>1503412276262</LastAccessedDate>
            <LoginAttempts>0</LoginAttempts>
            <TimeTrackingUser>false</TimeTrackingUser>
            <NoWorkDone>1446731581084</NoWorkDone>
            <PageSize>40</PageSize>
            <Status>ACTIVATED</Status>
            <AccountsAdministrator>true</AccountsAdministrator>
            <AddGroupings>true</AddGroupings>
            <NotifyMethod>EMAIL</NotifyMethod>
            <HrManager>true</HrManager>
            <TimeZone>36,GMT+02:00</TimeZone>
            <ReceiveDailyNotification>false</ReceiveDailyNotification>
            <ReceiveRealtimeNotifications>true</ReceiveRealtimeNotifications>
            <HideDetails>false</HideDetails>
            <TaskView>LIST</TaskView>
            <GroupingSignedView>STATUSLANE</GroupingSignedView>
            <GroupingUnsignedView>LIST</GroupingUnsignedView>
            <Type>SALES</Type>
            <RewardStatus>NONE</RewardStatus>
            <AnnualLeave>26</AnnualLeave>
            <SickLeave>0</SickLeave>
            <CompassionateLeave>0</CompassionateLeave>
            <OtherLeave>0</OtherLeave>
            <ReceiveHrEmails>true</ReceiveHrEmails>
            <HourCapacityPerDay>8.0</HourCapacityPerDay>
            <EmployeeCost>0.0</EmployeeCost>
            <CostEstimatePermission>WRITE_APPROVE</CostEstimatePermission>
            <PurchaseOrderPermission>WRITE</PurchaseOrderPermission>
            <TaxInvoicePermission>WRITE</TaxInvoicePermission>
            <SupplierInvoicePermission>WRITE</SupplierInvoicePermission>
            <ExpensePermission>NONE</ExpensePermission>
            <Active>true</Active>
            <FirstLastInitial>Oliver J</FirstLastInitial>
          </Author>
          <Winner>
            <Id>53090727</Id>
            <Version>200</Version>
            <Title>Studio Manager</Title>
            <FirstName>Oliver</FirstName>
            <LastName>Jeffery</LastName>
            <FullName>Oliver Jeffery</FullName>
            <Email>magnetic@email.co.uk</Email>
            <ContactNumber>07123456789</ContactNumber>
            <Description />
            <UserName>magnetic@email.co.uk</UserName>
            <RoleType>ADMIN</RoleType>
            <UserManager>true</UserManager>
            <Skin>bing</Skin>
            <Accounts>true</Accounts>
            <Grouping>Design</Grouping>
            <CreatedDate>1446813531845</CreatedDate>
            <LastAccessedDate>1503412276262</LastAccessedDate>
            <LoginAttempts>0</LoginAttempts>
            <TimeTrackingUser>false</TimeTrackingUser>
            <NoWorkDone>1446731581084</NoWorkDone>
            <PageSize>40</PageSize>
            <Status>ACTIVATED</Status>
            <AccountsAdministrator>true</AccountsAdministrator>
            <AddGroupings>true</AddGroupings>
            <NotifyMethod>EMAIL</NotifyMethod>
            <HrManager>true</HrManager>
            <TimeZone>36,GMT+02:00</TimeZone>
            <ReceiveDailyNotification>false</ReceiveDailyNotification>
            <ReceiveRealtimeNotifications>true</ReceiveRealtimeNotifications>
            <HideDetails>false</HideDetails>
            <TaskView>LIST</TaskView>
            <GroupingSignedView>STATUSLANE</GroupingSignedView>
            <GroupingUnsignedView>LIST</GroupingUnsignedView>
            <Type>SALES</Type>
            <RewardStatus>NONE</RewardStatus>
            <AnnualLeave>26</AnnualLeave>
            <SickLeave>0</SickLeave>
            <CompassionateLeave>0</CompassionateLeave>
            <OtherLeave>0</OtherLeave>
            <ReceiveHrEmails>true</ReceiveHrEmails>
            <HourCapacityPerDay>8.0</HourCapacityPerDay>
            <EmployeeCost>0.0</EmployeeCost>
            <CostEstimatePermission>WRITE_APPROVE</CostEstimatePermission>
            <PurchaseOrderPermission>WRITE</PurchaseOrderPermission>
            <TaxInvoicePermission>WRITE</TaxInvoicePermission>
            <SupplierInvoicePermission>WRITE</SupplierInvoicePermission>
            <ExpensePermission>NONE</ExpensePermission>
            <Active>true</Active>
            <FirstLastInitial>Oliver J</FirstLastInitial>
          </Winner>
          <DefaultBillable>NOTSET</DefaultBillable>
          <TimeWarning>NONE</TimeWarning>
          <GrossProfitFinancialWarning>NONE</GrossProfitFinancialWarning>
          <NetProfitFinancialWarning>NONE</NetProfitFinancialWarning>
          <Duration>3</Duration>
        </Grouping>
        <Owner>
          <Id>53090727</Id>
          <Version>200</Version>
          <Title>Studio Manager</Title>
          <FirstName>Oliver</FirstName>
          <LastName>Jeffery</LastName>
          <FullName>Oliver Jeffery</FullName>
          <Email>magnetic@email.co.uk</Email>
          <ContactNumber>07123456789</ContactNumber>
          <Description />
          <UserName>magnetic@email.co.uk</UserName>
          <RoleType>ADMIN</RoleType>
          <UserManager>true</UserManager>
          <Skin>bing</Skin>
          <Accounts>true</Accounts>
          <Grouping>Design</Grouping>
          <CreatedDate>1446813531845</CreatedDate>
          <LastAccessedDate>1503412276262</LastAccessedDate>
          <LoginAttempts>0</LoginAttempts>
          <TimeTrackingUser>false</TimeTrackingUser>
          <NoWorkDone>1446731581084</NoWorkDone>
          <PageSize>40</PageSize>
          <Status>ACTIVATED</Status>
          <AccountsAdministrator>true</AccountsAdministrator>
          <AddGroupings>true</AddGroupings>
          <NotifyMethod>EMAIL</NotifyMethod>
          <HrManager>true</HrManager>
          <TimeZone>36,GMT+02:00</TimeZone>
          <ReceiveDailyNotification>false</ReceiveDailyNotification>
          <ReceiveRealtimeNotifications>true</ReceiveRealtimeNotifications>
          <HideDetails>false</HideDetails>
          <TaskView>LIST</TaskView>
          <GroupingSignedView>STATUSLANE</GroupingSignedView>
          <GroupingUnsignedView>LIST</GroupingUnsignedView>
          <Type>SALES</Type>
          <RewardStatus>NONE</RewardStatus>
          <AnnualLeave>26</AnnualLeave>
          <SickLeave>0</SickLeave>
          <CompassionateLeave>0</CompassionateLeave>
          <OtherLeave>0</OtherLeave>
          <ReceiveHrEmails>true</ReceiveHrEmails>
          <HourCapacityPerDay>8.0</HourCapacityPerDay>
          <EmployeeCost>0.0</EmployeeCost>
          <CostEstimatePermission>WRITE_APPROVE</CostEstimatePermission>
          <PurchaseOrderPermission>WRITE</PurchaseOrderPermission>
          <TaxInvoicePermission>WRITE</TaxInvoicePermission>
          <SupplierInvoicePermission>WRITE</SupplierInvoicePermission>
          <ExpensePermission>NONE</ExpensePermission>
          <Active>true</Active>
          <FirstLastInitial>Oliver J</FirstLastInitial>
        </Owner>
        <Discount>0.0</Discount>
        <Archive>false</Archive>
        <Tag />
        <HideQtyAndCost>false</HideQtyAndCost>
        <ModifiedDate>1500993521166</ModifiedDate>
        <Currency>GBP</Currency>
        <ExchangeRate>1.0</ExchangeRate>
      </Account>
      <LineItems>
        <LineItem>
          <Id>54067399</Id>
          <Version>1</Version>
          <ItemType>
            <Id>54065742</Id>
            <Version>0</Version>
            <Name>Filming</Name>
            <ExternalName />
            <Cost>50.0</Cost>
            <TaxType>TAX</TaxType>
            <Markup>999.0</Markup>
            <Description>Filming</Description>
            <Company>
              <Id>53090725</Id>
              <Version>13</Version>
              <Name>Zynk Ltd</Name>
              <ContactPerson>Nathan Hopkins</ContactPerson>
              <ContactNumber>07123456789</ContactNumber>
              <EmailAddress>Nathan@Zynk.com</EmailAddress>
              <PhysicalAddress />
              <PostalAddress />
              <Website />
              <MailDomain />
              <DefaultSkin />
              <GroupingName>Project</GroupingName>
              <TotalSmsesSent>0</TotalSmsesSent>
              <TotalEmailsSent>0</TotalEmailsSent>
              <CreatedDate>1446813531845</CreatedDate>
              <Active>true</Active>
              <ReceiveEmailNotifications>true</ReceiveEmailNotifications>
              <Hr>true</Hr>
              <GroupingCodePrefix />
              <AccountsPrefix />
              <NotificationsActive>BOTH</NotificationsActive>
              <NotifyMethod>EMAIL</NotifyMethod>
              <RetentionPeriod>90</RetentionPeriod>
              <SignatureRecognition>UPDATECONTACTS</SignatureRecognition>
              <Accounts>true</Accounts>
              <Ical>true</Ical>
              <PricingPackage>FREE</PricingPackage>
              <CloseDate>1447970400000</CloseDate>
              <OnlyApprovedCompaniesInAccounts>false</OnlyApprovedCompaniesInAccounts>
              <UserRate>250.0</UserRate>
              <FreelancerRate>0.0</FreelancerRate>
              <FixedRate>0.0</FixedRate>
              <MaxMonthlyActiveUsers>7</MaxMonthlyActiveUsers>
              <MaxMonthlyActiveUserList>gtdemo@flowbird.co.uk,junior@creativenet.net,l@magneticdemo.net,copywriter@magnetichq.com,designer@magneticdemo.net,creative@magneticdemo.net,magnetic@flowbird.co.uk</MaxMonthlyActiveUserList>
              <MaxMonthlyActiveFreelancers>0</MaxMonthlyActiveFreelancers>
              <MaxMonthlyActiveFreelancerList />
              <GroupingCode>3486</GroupingCode>
              <TaxFree>false</TaxFree>
              <Country>GB</Country>
              <TaskItemTypeRequired>true</TaskItemTypeRequired>
              <BlockAccessTimesheetsNotFilled>true</BlockAccessTimesheetsNotFilled>
              <RecurringTasksEnabled>true</RecurringTasksEnabled>
              <PaymentTerms>30 Days,30 Days from Invoice,14 Days from Invoice,7 Days from Invoice,30 Days from Statement,50% deposit + Progress Payments,50% deposit + 50% on completion,60% deposit,66% deposit,75% deposit,Cash On Delivery,On Invoice,On Signing,Paid</PaymentTerms>
              <NoCostEstimateSendingDraft>false</NoCostEstimateSendingDraft>
              <TaxPercentage>20.0</TaxPercentage>
              <OpportunitiesBillable>NOTSET</OpportunitiesBillable>
              <AccountsFooterText />
              <GroupAccountLineItems>false</GroupAccountLineItems>
              <AccountIntegrationType>NONE</AccountIntegrationType>
              <CostEstimatesIntegrationType>NONE</CostEstimatesIntegrationType>
              <PurchaseOrdersIntegrationType>NONE</PurchaseOrdersIntegrationType>
              <RevenueIntegrationType>NONE</RevenueIntegrationType>
              <BaseCurrency>GBP</BaseCurrency>
              <OnlyCreateAccountsOffCostEstimate>false</OnlyCreateAccountsOffCostEstimate>
              <BudgetWarningLevel>0.75</BudgetWarningLevel>
            </Company>
            <BillableByDefault>false</BillableByDefault>
            <Archive>false</Archive>
            <ArchivedDate>0</ArchivedDate>
            <CreatedDate>1447764570449</CreatedDate>
          </ItemType>
          <RefCode>53130779</RefCode>
          <Unit>10.0</Unit>
          <Cost>50.0</Cost>
          <Markup>999.0</Markup>
          <Ordering>0</Ordering>
          <TaxType>TAX</TaxType>
          <Notes>Filming</Notes>
          <DocType>TAX_INVOICE</DocType>
        </LineItem>
      </LineItems>
    </TaxInvoice>
  </TaxInvoices>
  <Total>1</Total>
</MagneticHQData>
```
