# SwiftFirst
First Swift code upload
Hi, this is my HackingWithSwift tasks + some additional ones. 
//CHECKPOINT 6
struct Car {
    let model: String
    let numberSeats: Int
    public var gear = 1
    enum Gear {
        case up, down, neutral
    }
    public mutating func changeGear(_ direction: Gear){
        switch direction {
        case .down: gear -= 1
            if gear < 1 {gear = 1}
        case .up: gear += 1
            if gear > 10 {gear = 10}
        case .neutral:
            gear = 1
        }
        print("The \(model) is in gear \(gear)")
    }
}
var test = Car(model: "Audi", numberSeats: 5, gear: 1)
test.changeGear(.up)
test.changeGear(.down)
test.changeGear(.neutral)

February 6:
DId code which does not work, require more effort while working on problems
//did not work
struct Business {
    var model: String
    var income: String
    public(set) var amountHaving: Double
}
enum Cases {
    case highAmount, moderateAmount, lowAmount
}
func checkAmount(_ amount: Cases) {
    switch amount {
     case .highAmount:
        if .highAmount > 1000 {
            print("Suggested: Retail Store")
        }
    case .moderateAmount {
        if .moderateAmount.range(1...500) {
            print("Try Dropshipping")
        }
    case .lowAmount {
        if .lowAmount < 100 {
            print("Try to gain using crypto")
        }
    }
    }
    }
}
var check = Business(model: "StartUp", income: "Moderate", amountHaving: 15555.0)
print(.highAmount)
print(.moderateAmount)
print(.lowamount)
