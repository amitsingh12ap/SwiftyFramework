# SwiftyFramework

Add this framework in Embedded Binaries. 
import SwiftyService

Use below code to call your api.

let service = SwiftyApiManager(configuration: .default)

 service.connectApi(withEndPoint: urlString, withRequestType: .get, withParameters: nil, withHeader: nil, decode: yourcodeableprotocl.self) { (response) in
            switch response {
                case .success(let codableModel):
                    print("\(codableModel)")
                case .failure(let failure):
                    print("Failed ")
            }
}



