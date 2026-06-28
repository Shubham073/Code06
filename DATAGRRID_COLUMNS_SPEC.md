# DataGrid Column Specifications

## 1. Purchase Orders List Grid (PurchaseOrders.tsx)
### PO List Columns (Default Tab)
- **po_number** - PO Number (width: TBD)
- **po_version** - Version (width: TBD)
- **supplier_name** - Supplier Name (width: TBD)
- **po_status** - Status (width: TBD)
- **total_value** - Total Value (width: TBD)
- **delivery_date** - Delivery Date (width: TBD)
- **procurement_specialist_name** - Procurement Specialist (width: TBD)
- **pin** - Pin icon (width: 60)
- **actions** - Actions menu (width: 58) [NEW]

### Line Item Columns (PO To Review / MRP Exception Tabs)
#### Supplier Collaboration Context (Exceptions & Alerts / Action Required Tabs)
- **pin** - Pin icon (width: 60)
- **po_line** - PO Line (width: 84)
- **material_code** - Material No (width: 108)
- **line_status** - Status (width: 60)
- **description** - Short Description (flex: 1, width: 200)
- **quantity** - Qty (width: 64)
- **unit** - UOM (width: 58)
- **unit_price** - Unit Price (width: 86)
- **net_value** - Total Value (width: 96)
- **required_in_house_date** - Need By Date (width: 100) [Urgency coloring for Supplier Collaboration]
- **actions** - Action menu (width: 58) [NEW in PurchaseOrderDetails]

#### Cockpit Context (Ready to Review / MRP Exception Tabs)
- **pin** - Pin icon (width: 60)
- **po_line** - PO Line (width: 84)
- **material_code** - Material No (width: 108)
- **line_status** - Status (width: 60)
- **description** - Short Description (flex: 1, width: 200)
- **quantity** - Qty (width: 64)
- **updated_quantity** - Supplied Qty (width: 84)
- **unit** - UOM (width: 58)
- **unit_price** - Unit Price (width: 86)
- **updated_unit_price** - Updated Unit Price (width: 80)
- **net_value** - Total Value (width: 96)
- **updated_net_value** - Updated Total Value (width: 60)
- **updated_total** - Updated Total (width: 60)
- **required_in_house_date** - Need By Date (width: 100)
- **updated_delivery_date** - Revised Date (width: 100)
- **supplier_confirmation** - Supplier Confirmation (width: 60)
- **concession** - Concession link (width: 90) [Clickable in Cockpit context]
- **actions** - Action menu (width: 58) [NEW]

## 2. Documents Grid
- **file_name** - Document Name
- **file_type** - Document Type
- **uploaded_date** - Upload Date
- **uploaded_by** - Uploaded By
- **action** - Review/Accept/Reject actions

## 3. History Grid
- **event_type** - Event Type
- **changed_by** - Changed By
- **timestamp** - Timestamp
- **change_details** - Change Details

## Notes
- [NEW] indicates columns that were added in this feature implementation
- All widths are in pixels except where marked with 'flex'
- Supplier Collaboration has special formatting for need-by-date urgency (red for past-due, orange for within 30 days)
- Cockpit shows updated values alongside original values for comparison
- Action columns appear only in specific tab contexts
