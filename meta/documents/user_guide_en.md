<div class="alert alert-warning" role="alert">
   <strong><i>Note:</i></strong> The Novalnet plugin has been developed for use with the online store Ceres and only works with its structure or other template plugins. IO plugin is required.
</div>

### Long description:

# Novalnet payment plugin for plentymarkets

Novalnet's payment plugin for plentymarkets is an end-to-end solution for accepting both international and local payments across the world. This full-service payment plugin automates your entire payment processing through one single PCI certified payment platform including the following benefits and more:
- End-to-end payment solution incl. 15+ automated payment services (e.g. debt collection, fraud prevention) 
- Accept and process 100+ international and local payment methods
- One contract - no hidden costs or restrictive contract terms for payment processing
- PCI compliance (PCI DSS Level 1) & extensive payment licensing ready for you
- Professional customer support on many levels (e.g. merchant + buyer support) directly in-house

The Novalnet payment plugin integrates your business with the BaFin (German Federal Financial Supervisory Authority) accredited Novalnet payment platform and eliminates the need of multiple contracts and licenses for successful payment processing. Streamline your payment processes and focus on your core businesses' growth!

## Supported Novalnet payment methods

- Credit Card (3DSecure and non 3DSecure)
- Direct Debit SEPA
- Direct Debit SEPA with payment guarantee
- Invoice
- Invoice with payment guarantee
- Prepayment
- Instant Bank Transfer
- iDEAL
- PayPal
- giropay
- eps
- Przelewy24
- Barzahlen

## Opening a Novalnet merchant account

To accept and process payments via the Novalnet payment plugin for plentymarkets, you need to have a Novalnet merchant account. You can get your account by contacting us either by phone at +49 89 9230683-20 or by email at sales@novalnet.de. More information about the Novalnet merchant account can be found at www.novalnet.com

## Configuring Novalnet in plentymarkets

To set up the merchant credentials, navigate to the path **Plugins -> Plugin overview -> Novalnet -> Configuration**

Fill in your Novalnet merchant account details as follows:
1. Login into your merchant account at [Novalnet Merchant Administration Portal](https://admin.novalnet.de/)
2. Navigate to the tab **PROJECT**
3. Select the corresponding product
4. Go to Shop Parameters and copy the necessary fields such as **Merchant ID**, **Authentication code**, **Project ID**, **Tariff ID** and **Payment access key** etc.

<table>
    <thead>
        <th>
            Setting
        </th>
        <th>
            Description
        </th>
    </thead>
    <tbody>
        <tr>
        <td class="th" align=CENTER colspan="2">General</td>
        </tr>        
        <tr>
            <td><b>Merchant ID</b></td>
            <td>Enter your merchant number that you received after opening a merchant account at Novalnet. Please contact Novalnet at <a href="mailto:sales@novalnet.de" target="_blank">sales@novalnet.de</a> for getting your own merchant account.</td>
        </tr>
        <tr>
            <td><b>Authentication code</b></td>
            <td>Enter your merchant password (authentication code) received after opening a merchant account at Novalnet.</td>
        </tr>
        <tr>
            <td><b>Project ID</b></td>
            <td>A unique identification number of a project created at the <a href="https://admin.novalnet.de/" target="_blank">Novalnet Merchant Administration Portal.</a></td>
        </tr>
        <tr>
            <td><b>Tariff ID</b></td>
            <td>Tariff ID is a unique identifier for the created tariff plan. Select the required Tariff ID to make sure that proper Tariff ID is used for this project.</td>
        </tr>
        <tr>
            <td><b>Payment access key</b></td>
            <td>Secure public key for encryption and decryption of transaction parameters. This is mandatory value for all online transfers, Credit Card-3D secure and wallet systems. </td>
        </tr>
    </tbody>
</table>

## Novalnet Payment configuration in plentymarkets

To activate the preferred payment methods, sign into the [Novalnet Merchant Administration Portal](https://admin.novalnet.de/).

1. Navigate to the tab **PROJECT**
2. Select the corresponding product
3. **Payment Methods**
4. **Edit Payment Methods**. 

For more detailed information, please follow the **Novalnet Payment Plugin Installation Guide for Plentymarkets** with explanatory screenshots for all payment settings. The installation guide is included in the plugin package that you download.

## Event creation for confirm/cancel/refund transactions

To set up an event procedure to confirm, cancel or refund Novalnet transactions:Set up an event procedure to Confirm, Cancel and Refund the Novalnet transactions:

1. Go to **System » Orders » Events**.
2. Click on **Add event procedure**. <br > → The **Create new event procedure** window opens.
3. Enter a name.
4. Select the event according to tables 1-3.
5. **Save** the settings. <br > → The event procedure is created.
6. Carry out the further settings according to tables 1-3.
7. Place a check mark next to the option **Active**.
8. **Save** the settings. <br > → The event procedure is saved. 

<table>
   <thead>
    </tr>
      <th>
         Setting
      </th>
      <th>
         Option
      </th>
      <th>
         Selection
      </th>
    </tr>
   </thead>
   <tbody>
      <tr>
         <td><strong>Event</strong></td>
         <td>Select the event to trigger a confirm procedure.</td>
         <td></td>
      </tr>
      <tr>
         <td><strong>Filter 1</strong></td>
         <td><strong>Order > Payment method</strong></td>
         <td><strong>Plugin: Novalnet Invoice</strong></td>
      </tr>
      <tr>
        <td><strong>Procedure</strong></td>
        <td><strong>Plugins > Novalnet | Confirm</strong></td>
        <td></td>
      </tr>
    </tbody>
    <caption>
    Table 1: Event procedure to confirm Novalnet transaction
    </caption>
</table>


<table>
   <thead>
    </tr>
      <th>
         Setting
      </th>
      <th>
         Option
      </th>
      <th>
         Selection
      </th>
    </tr>
   </thead>
   <tbody>
      <tr>
         <td><strong>Event</strong></td>
         <td>Select the event to trigger a cancel procedure.</td>
         <td></td>
      </tr>
      <tr>
         <td><strong>Filter 1</strong></td>
         <td><strong>Order > Payment method</strong></td>
         <td><strong>Plugin: Novalnet Invoice</strong></td>
      </tr>
      <tr>
        <td><strong>Procedure</strong></td>
        <td><strong>Plugins > Novalnet | Cancel</strong></td>
        <td></td>
      </tr>
    </tbody>
    <caption>
    Table 2: Event procedure to cancel Novalnet transaction
    </caption>
</table>


<table>
   <thead>
    </tr>
      <th>
         Setting
      </th>
      <th>
         Option
      </th>
      <th>
         Selection
      </th>
    </tr>
   </thead>
   <tbody>
      <tr>
         <td><strong>Event</strong></td>
         <td>Select the event to trigger a refund procedure.</td>
         <td></td>
      </tr>
      <tr>
         <td><strong>Filter 1</strong></td>
         <td><strong>Order > Payment method</strong></td>
         <td><strong>Plugin: Novalnet Invoice</strong></td>
      </tr>
      <tr>
        <td><strong>Procedure</strong></td>
        <td><strong>Plugins > Novalnet | Refund</strong></td>
        <td></td>
      </tr>
    </tbody>
    <caption>
    Table 3: Event procedure to refund Novalnet transaction
    </caption>
</table>

## Displaying the payment transaction details on the invoice pdf

Generating invoice for the orders to display the payment transaction details in invoice pdf except for the initial order created events.

## Displaying the payment transaction details on the order confirmation page

To display the payment transaction details on the order confirmation page, perform the steps as follows.

##### Displaying transaction details:

1. Go to **CMS » Container links**..
3. Go to the **Novalnet payment details** area.
4. Activate the container **Order confirmation: Additional payment information**.
5. **Save** the settings.<br />→ The payment transaction details will be displayed on the order confirmation page.

## Update of Vendor Script URL

Vendor script URL is required to keep the merchant’s database/system up-to-date and synchronized with Novalnet transaction status. It is mandatory to configure the Vendor Script URL in [Novalnet Merchant Administration Portal](https://admin.novalnet.de/).

Novalnet system (via asynchronous) will transmit the information on each transaction and its status to the merchant’s system.

To configure Vendor Script URL,

1. Login into your merchant account.
2. Navigate to the tab **PROJECTS**.
3. Select the corresponding product.
4. Under the tab **Project Overview**.
5. Set up the **Vendor script URL** fof your store. In general the vendor script URL will be like **YOUR SITE URL/payment/novalnet/callback**.

## Further reading

To know more information about the Novalnet and it's features, please contact at  [sales@novalnet.de](mailto:sales@novalnet.de)
