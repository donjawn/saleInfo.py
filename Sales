# Sales Sheet


# functions
def GoatSale(salePrice): # calculates Goat App fees
    goatFees = (salePrice * 0.095) + 5
    return goatFees


def ppFees(grossSale): # calulates Paypal fees
    paypalFees = (grossSale * 0.029) + 0.30
    return paypalFees


def stockxSale(salePrice): # calculates StockX fees
    stockxFee1 = salePrice * 0.09
    stockxFee2 = salePrice * 0.03
    stockxTotalFees = stockxFee1 + stockxFee2
    return stockxTotalFees

def ebaySale(salePrice): # calculates eBay fees2
    ebayFee = salePrice * 0.10
    return ebayFee



# main
print
purchasePrice = float(raw_input("How much did the shoes cost?: "))
print
salePrice = float(raw_input("How much did you sell the shoes for?: "))
print
forwarder = raw_input("Did you use a forwarder? Enter 'Yes' or 'No': ").lower()
if forwarder == 'yes':
    forwarderFee = float(raw_input("How much did it cost to forward the shoes?: "))
else:
    platform = raw_input("On what platform did you sell them? Goat, StockX, eBay, or Paypal?: ").lower()
    if platform == 'goat':
        print "The total amount of fees from Goat are", GoatSale(salePrice)
        print
        fees1 = GoatSale(salePrice) # fees just from Goat
        grossSale = salePrice - fees1 # amount after Goat takes their cut 
        print "The total amount of fees from Paypal are", ppFees(grossSale)
        print
        fees2 = ppFees(grossSale)
        payOut = salePrice - (fees1 + fees2) # amount after Goat and Paypal take their cuts
        profitSale = payOut - purchasePrice
        print "After the fees from Goat and Paypal are removed, the shoes were ultimately sold for", payOut, "for a \n total profit of", profitSale
    elif platform == 'stockx':
        print "The total amount of fees from StockX are", stockxSale(salePrice)
        print
        fees3 = stockxSale(salePrice) # fees just from StockX
        payOut1 = salePrice - fees3 # amount after StockX takes their cut
        profitSale1 = payOut1 - purchasePrice
        print "After the fees from StockX are removed, the shoes were ultimately sold for", payOut1, "for a \n total profit of", profitSale1
    elif platform == 'ebay':
        print "The total amount of fees from eBay are", ebaySale(salePrice) # fees just from eBay
        print
        grossSale = salePrice
        print "The total amount of fees from Paypal are", ppFees(grossSale) # fees just from paypal 
        total_ebayFee = ebaySale(salePrice) - ppFees(grossSale) # amount of fees from BOTH paypal and eBay
        payOut2 = salePrice - total_ebayFee
        print
        shippingFee = float(raw_input("How much did it cost to ship? ")) # fees from shipping
        payOut3 = payO250ut2 - shippingFee # total payout after eBay, Paypal, and shipping fees
        profitSale2 = payOut3 - purchasePrice
        print "After the fees from eBay and Paypal are removed and you pay for shipping, the shoes were ultimately sold for", payOut3, "for a \n total profit of", profitSale2
    elif platform == 'paypal':
        paymentType = raw_input("Was it an 'Invoice' or 'Gift'? ").lower()
        if paymentType == 'invoice':
            print "The total amount of fees from Paypal are", ppFees(grossSale) # fees just from paypal
            shippingFee1 = float(raw_input("How much did it cost to ship? "))
            total_ppFee = ppFees(grossSale) - shippingFee1 # invoice fee and shipping charge added together
            payout4 = salePrice - total_ppFee # payout after invoice and shipping fee
            profitSale3 = payOut4 - purchasePrice # profit
            print
            print " After the fees from Paypal are removed and you pay for shipping, the shoes were ultimately sold for", payOut4, "for a \n total profit of", profitSale3
        elif paymentType == 'gift':
            shippingFee2 = float(raw_input("How much did it cost to ship? "))
            payOut5 = salePrice - shippingFee2 # payout after shipping fee
            profitSale4 = payOut5 - purchasePrice # profit
            print
            print "After you pay for shipping, the shoes were ultimately sold for", payOut5, "for a \n total profit of", profitSale4
            print

print "Congratulations on the sale! This is money you didn't have before...unless it's a brick."
        
        
                        
                            
        
        
        
        
