# π°π· λ§κ΅­λ°λν

## π λͺ©μ°¨
1. [μκ°](#-μκ°)
2. [Tree](#-tree)
3. [κ³ λ―Όν μ ](#-κ³ λ―Όν-μ )
4. [νμλΌμΈ](#-νμλΌμΈ)
5. [μ€ν νλ©΄](#-μ€ν-νλ©΄)
6. [νΈλ¬λΈ μν](#-νΈλ¬λΈ-μν)
7. [μ°Έκ³  λ§ν¬](#-μ°Έκ³ -λ§ν¬)

## π± μκ°

`Hamo`μ `mene` κ° λ§λ  λ§κ΅­λ°λν μ±μλλ€.

- JSONμ λμ½λ©νμ¬ 1900 λ§κ΅­λ°λν μ λ³΄λ₯Ό TableView νλ©΄μ λ³΄μ¬μ€λλ€.
- λ©μΈ νλ©΄κ³Ό νκ΅­μ μΆνμ λͺ©λ‘, μμΈνλ©΄μΌλ‘ κ΅¬μ±λμ΄ μμ΅λλ€.
- **KeyWords**
  - `UITableView`
      - `UITableViewDataSource`, `UITableViewDeligate`, `prepareforreuse`
  - `JSON`
      - `DTO`, `CodingKey`, `keyDecodingStrategy`, `convertFromSnakeCase`
      - `Codable`, `Encodable`, `Decodable`
  - `NSMutableAttributedString`
  - `Accessbility`
      - `Dynamic Type`


## π» κ°λ°νκ²½ λ° λΌμ΄λΈλ¬λ¦¬
[![swift](https://img.shields.io/badge/swift-5.6-orange)]()
[![xcode](https://img.shields.io/badge/Xcode-13.4.1-blue)]()


## π§ νμ
<img src = "https://avatars.githubusercontent.com/u/84453688?v=4" width=160>|<img src="https://i.imgur.com/ydRkDFq.jpg" width=200>|
|:--:|:--:|
|[Mene](https://github.com/JaeKimdev)|[νλͺ¨](https://github.com/lxodud)|

## π² Tree

```
βββ Expo1900
βΒ Β  βββ ExhibitionEntryTests
βΒ Β  βββ Expo1900
βΒ Β  βΒ Β  βββ AppDelegate.swift
βΒ Β  βΒ Β  βββ Assets.xcassets
βΒ Β  βΒ Β  βΒ Β  βββ Contents.json
βΒ Β  βΒ Β  βΒ Β  βββ expo_assets
βΒ Β  βΒ Β  βββ Base.lproj
βΒ Β  βΒ Β  βΒ Β  βββ LaunchScreen.storyboard
βΒ Β  βΒ Β  βββ Controller
βΒ Β  βΒ Β  βΒ Β  βββ EntryDetailViewController.swift
βΒ Β  βΒ Β  βΒ Β  βββ ExpositionUniverselleViewController.swift
βΒ Β  βΒ Β  βΒ Β  βββ KoreanEntriesViewController.swift
βΒ Β  βΒ Β  βββ Extensioin
βΒ Β  βΒ Β  βββ Info.plist
βΒ Β  βΒ Β  βββ Model
βΒ Β  βΒ Β  βΒ Β  βββ ExhibitionEntry.swift
βΒ Β  βΒ Β  βΒ Β  βββ ExpoConstant.swift
βΒ Β  βΒ Β  βΒ Β  βββ ExpoError.swift
βΒ Β  βΒ Β  βΒ Β  βββ ExpositionUniverselle.swift
βΒ Β  βΒ Β  βΒ Β  βββ JSONDecodingManager.swift
βΒ Β  βΒ Β  βββ SceneDelegate.swift
βΒ Β  βΒ Β  βββ View
βΒ Β  βΒ Β      βββ Base.lproj
βΒ Β  βΒ Β      βΒ Β  βββ Main.storyboard
βΒ Β  βΒ Β      βββ EntryTableViewCell.swift
βββ README.md
```
 
## π κ³ λ―Όν μ 

### Step 1

- Codable νλ‘ν μ½μ μ±νν μ§, Decodableλ§ μ±νν μ§ κ³ λ―Όν΄ λ³΄μμ΅λλ€.
    - μ΄λ² νλ‘μ νΈμμλ Encodingμ΄ νμνμ§ μμκ³  λ€λ₯Έ μ¬λμ΄ λ³΄μμ λμλ λͺννκ² Decodingλ§ νλ νλ‘μ νΈλΌλ κ²μ μ μ μκ² λκΈ° λλ¬Έμ λͺ¨λΈνμμ Decodableλ§μ μ±ννμμ΅λλ€.
- Namingμ, νμ₯μ±μ κ³ λ €νμμ΅λλ€.
    - μ§κΈμ `1900λ Expo`μ μ λ³΄λ§ μ‘΄μ¬νμ§λ§ μΆν λ€λ₯Έ λλμ Expoκ° μΆκ°λ  μλ μμ§ μμκΉ?λΌλ μκ°μ ν΄ λ³΄μκ³  `νκ΅­μ μΆνμ` μ­μ λ€λ₯Έ μ°Έκ°κ΅­μ μ λ³΄κ° μΆκ°λ  κ°λ₯μ±μ΄ μμ΄ νμ₯μ±μ κ³ λ €νμ¬ `ExpositionUniverselle`κ³Ό `ExhibitionEntry`λ‘ μ§μ νμμ΅λλ€.

### Step 2

- λ©μΈνμ΄μ§μ Titleμ κ΅¬μ±ν  λ labelκ³Ό textViewμ€μ μ΄λ€ κ²μ μ¬μ©ν  μ§ κ³ λ―Όν΄ λ³΄μμ΅λλ€.
    - Labelμ κ²½μ° numberOfLinesλ₯Ό 0μΌλ‘ ν λΉνμ¬ μ¬λ¬μ€μ νμ€νΈλ₯Ό ννν  μ μμ΅λλ€.
    - [textView κ³΅μλ¬Έμ](https://developer.apple.com/library/archive/documentation/StringsTextFonts/Conceptual/TextAndWebiPhoneOS/UsingTextClasses/UsingTextClasses.html)μμ large amounts of textλ₯Ό μ¬μ©ν  λλ textViewλ₯Ό μ¬μ©νλΌκ³  λμ΄μμ΄μ `editable`, `scrolling enabled`λ₯Ό ν΄μ νκ³  textViewλ₯Ό μ¬μ©νμμ΅λλ€.
- λ°©λ¬Έκ°, κ°μ΅μ§, κ°μ΅κΈ°κ° λ± νμ€νΈ νΉμ  λΆλΆλ§ μ¬μ΄μ¦λ₯Ό λ€λ₯΄κ² λ³΄μ¬μ£ΌκΈ° μν΄ κ³ λ―Όν΄ λ³΄μμ΅λλ€.
    - ν΄λΉ λΆλΆμ κ΅¬ννκΈ° μν΄ labelμ 2κ°λ‘ λΆλ¦¬νμ¬ λ°λ‘ νμνλ λ°©λ²κ³Ό attributedTextλ₯Ό μ΄μ©ν΄μ νΉμ  λ¬Έμμ΄μ μμ±μ λΆμ¬νλ λ°©λ²μ΄ μμμ΅λλ€.
    - `attributedString`μ λν΄ κ³΅λΆν΄ λ³΄κ³  μ΄λ² νλ‘μ νΈμ μ μ©ν΄λ³΄κ³  μΆμ΄μ μ¬μ©νμμ΅λλ€.
- λ¬Έμμ΄ "λ°©λ¬Έκ° : ~λͺ"μ "λ°©λ¬Έκ°" + expositionUniverselle.formattedVisitor + "λͺ"μΌλ‘ λ§λλ κ²μ΄ κ°λμ±μ΄ μ’μ§ μμμ΅λλ€.
    - μ΄ λ¬Έμ λ₯Ό computed propertyλ₯Ό μ΄μ©νμ¬ ν΄κ²°νμμ΅λλ€.
- ν νλ©΄μμ λ€λΉκ²μ΄μ λ°λ₯Ό λΈμΆλμ§ μκ² νλ λ°©λ²μ κ³ λ―Όν΄ λ³΄μμ΅λλ€.
- λ°©λ¬Έκ° μ«μλ₯Ό λ³΄μ¬μ€ λ Numberformatterλ₯Ό μ¬μ©νμ¬ `,`λ₯Ό μΆκ°νμ¬ μ£Όμλλ°, μ¬λ¬λ² νΈμΆνλ κ²½μ° λ§€λ² κ°κ°μ μΈμ€ν΄μ€λ₯Ό μμ±ν΄μΌ ν΄μ μ±κΈν€ ν¨ν΄μΌλ‘ λ§λ€μ΄μΌ νλμ§ κ³ λ―Όν΄ λ³΄μμ΅λλ€.
    - μ΄λ² νλ‘μ νΈμμλ μμ§κΉμ§λ νλ²λ§ μ¬μ©λκ³  μμ΄μ μ±κΈν΄μΌλ‘ νμΌλΆλ¦¬ ν  νμλ μλ κ² κ°μ λ©μλλ‘ κ΅¬ννμμ΅λλ€.

### Step 3

- μ²«λ²μ§Έ λ·°λ§ μΈλ‘λͺ¨λλ‘ κ³ μ νκΈ° μν λ°©λ²μ κ³ λ―Όν΄ λ³΄μμ΅λλ€.
    - delegateλ₯Ό selfλ‘ μ§μ νμ¬ μ¬μ μν `supportedInterfaceOrientations`λ₯Ό λ¦¬ν΄νμ¬ κ° λ·°μμ μ¬μ©νλ λ°©λ²κ³Ό AppDelegateμ `UIInterfaceOrientationMask`λ₯Ό μ¬μ©νλ λ°©λ², UINavigationControllerμ subClassλ₯Ό κ΅¬ννμ¬ `supportedInterfaceOrientations`λ₯Ό μ¬μ μνλ λ°©λ² μ€ μ΄λ€ κ²μ μ¬μ©ν  μ§ κ³ λ―Όνμ΅λλ€.

- AttributedStringμ Dynamic Type μ μ©μ νμͺ½λ§ μ μ©λλ λ¬Έμ κ° μμ΄ ν΄κ²°λ°©λ²μ κ³ λ―Όν΄ λ³΄μμ΅λλ€.
    - Dynamic Typeμ μ μ©νκ³  νμΈν΄ λ³΄λ AttributedStringμ΄ μ μ©λ Textμλ§ Dynamic Typeμ΄ μ μ©λκ³  λ€μͺ½ Textμλ μ μ©λμ§ μλ λ¬Έμ κ° μμ΄ ν΄κ²°λ°©λ²μ μ°ΎκΈ° μν΄ κ³ λ―Όν΄ λ³΄μμ΅λλ€.

- description λ μ΄λΈμμ λ¨μ΄ λ¨μλ‘ μ€λ°κΏ λλλ‘ κ³ λ―Όν΄ λ³΄μμ΅λλ€.
    -  Labelμ lineBreakλ₯Ό `Word Wrap`μΌλ‘ μ€μ νμ¬ μ£Όμμ΅λλ€.
    -  iOS 14 μ΄μμμ μ μ©ν  μ μλ `lineBreakStrategy`μ `hangulWordPriority`λ ν¨κ» κ³΅λΆνμμΌλ μ΄λ² νλ‘μ νΈμλ μ μ©νμ§λ μμμ΅λλ€.

- μ²«λ²μ§Έ View νλ¨ `νκ΅­μ μΆνμ λ³΄λ¬κ°κΈ°` λ²νΌμ Dynamic Type μ μ©μ μ€νλ·° λ°κΉ₯μΌλ‘ λ²μ΄λλ λ¬Έμ  ν΄κ²°μ μν΄ κ³ λ―Όν΄ λ³΄μμ΅λλ€.
    - ν΄λΉ λ²νΌμ΄ μν΄μλ μ€νλ·°μ λμ΄κ° 50μΌλ‘ μ§μ λμ΄ μμ΄, Dynamic Typeλ₯Ό μ μ©νμ λ νμ€νΈκ° λ²νΌμ μ¬μ΄μ¦λ₯Ό λ²μ΄λλ λ¬Έμ κ° μμμ΅λλ€.
    - μ΄ λ¬Έμ λ₯Ό ν΄κ²°νκΈ° μν΄μ λ²νΌμ `Hugging Priority`λ₯Ό 1000μΌλ‘ μ£Όμ΄μ λμ΄λμ§ μλλ‘ νμ¬ ν΄κ²°νμμ΅λλ€.

- TableViewCellμ μ¬μ¬μ©μ μν identifierλ₯Ό UITalbeViewCellμ νμ νλ‘νΌν°λ‘ κ΅¬ννκΈ° μν΄ κ³ λ―Όν΄ λ³΄μμ΅λλ€.
    - TableViewCellμ μ¬μ¬μ©ν  λ μμ±νλ cell identifierλ₯Ό String literalμ΄ μλ λ€λ₯Έ λ°©μμΌλ‘ κ΅¬ννλ λ°©λ²μ λν΄ κ³ λ―Όνμμ΅λλ€.
    - String literalμ μ¬μ©νμ κ²½μ° ν΄λΉ Cell νμμ΄ μ¬λ¬λ² μ¬μ©λμμ λ μ μ§λ³΄μμΈ‘λ©΄μμ μ’μ§μκ³ , human errorλ₯Ό μ λ°ν  κ°λ₯μ±λ μ‘΄μ¬νλ€κ³  μκ°λ©λλ€.
    - κ° TableViewCellμ νμνλ‘νΌν°λ‘ identifierλ₯Ό λ¦¬ν΄νλ computed propertyλ₯Ό κ΅¬ννκ³  identifierλ₯Ό ν΄λμ€μ λ€μ΄λ°μΌλ‘ νλ λ°©λ²μ μ¬μ©ν΄λ³΄μμ΅λλ€.
        ```swift
        final class EntryTableViewCell: UITableViewCell {
            static var reuseIdentifier: String {
                return String(describing: self)
            }
        ```
    - λ§μ½μ μ¬μ¬μ©λ  Viewκ° λ λ§μμ‘μ λ identifierκ° νμν λͺ¨λ  νμμ computed propertyλ₯Ό κ΅¬νν΄μ£ΌκΈ° λ³΄λ€ νλ‘ν μ½μ μ΄μ©νλ λ°©λ²λ κ³ λ―Όν΄λ³΄μμ΅λλ€.
        ```swift
        protocol Reusable { }

        extension Reusable where Self: UIView {
            static var reuseIdentifier: String {
                return String(describing: self)
            }
        }

        extension UITableViewCell: Reusable { }
        ```
    - μ΄λ² νλ‘μ νΈμμλ νλμ νμ΄λΈ λ·°λ§ μ¬μ©νκ³  μμ΄ ν΄λΉ μμμ΄ μ€λ²μμ§λμ΄λ§μ΄λΌκ³  μκ°λμ΄ μ μ©νμ§ μμμ΅λλ€.

- EntryDetailViewControllerμ initializer κ΅¬ν
    - EntryDetailViewControllerμμ μ¬μ©ν  λ°μ΄ν°λ₯Ό λ΄κ³ μλ νλ‘νΌν°λ€μ κ΅¬νλΆκ° μλμ κ°μμ΅λλ€.
        ```swift
        var entryImage: UIImage?
        var entryDescription: String?
        ```
    - λ¬Έμ λ μΈλΆμμ ν΄λΉ νλ‘νΌν°μ μ κ·Όν΄μ κ°μ ν λΉν΄μ£Όλ κ²μ΄μμ΅λλ€. μ΄λ κ°μ²΄μ§ν₯μ μΌλ‘ μ’μ§μμ λ°©λ²μ΄λΌκ³  μκ°λμ΄ νλ‘νΌν°μ μ§μ  μ κ·Όνμ§μκ³  λ©μλλ₯Ό ν΅ν΄μ ν΄λΉ νλ‘νΌν°μ κ°μ μ§μ ν΄ μ£Όλκ² λ μ’λ€κ³  μκ°νμμ΅λλ€.
        ```swift
        func setupData(image: UIImage, description: String) {
            entryImage = image
            entryDescription = description
        }
        ```
    - μ¬κΈ°μ λ κ°μ§κ° λ λμ λμλλ° `var`μ `μ΅μλ`μ΄μμ΅λλ€. ν΄λΉ Viewμμ λ°μ΄ν°λ₯Ό λ΄κ³ μλ νλ‘νΌν°λ€μ νλ² ν λΉλκ³  κ°μ΄ λ³ν μΌμ΄ μλ μμμλλ€. <br>μ¬κΈ°μ `var`μ `optional`μ μ¬μ©ν μ΄μ λ κ°μ μΈλΆμμ ν λΉνλ μμ μ΄ μ΄κΈ°νλ¨κ³κ° μλκΈ° λλ¬Έμ μ΅μλμ μ΄μ©ν΄μ μ΄κΈ°κ°μ nilλ‘ ν λΉν΄μ£Όκ³  μ΄νμ κ°μ ν λΉν΄μ£ΌκΈ° μν΄μ varλ‘ μ μΈν κ²μ΄μμ΅λλ€.<br>κ·Έλ¬λ©΄ μ΄κΈ°ν μμ μμ νλ‘νΌν°μ κ°μ ν λΉν΄μ€λ€λ©΄ μ΅μλκ³Ό varλ₯Ό `let`μΌλ‘ λ°κΏμ€ μ μλ€κ³  μκ°λμ΄ initializerλ₯Ό κ΅¬ννκ³  μ¬μ©νμμ΅λλ€.
        ```swift
        // κ΅¬νν μ΄λμλΌμ΄μ 
        init?(entryInformation: ExhibitionEntry, coder: NSCoder) {
            self.entryInformation = entryInformation
            super.init(coder: coder)
        }
        ```
        ```swift
        // ν΄λΉ ViewController μΈμ€ν΄μ€ν
        guard let entryDetailViewController = storyboard?.instantiateViewController(
                identifier: "EntryViewController",
                creator: { coder in
                    return EntryDetailViewController(entryInformation: self.koreanEntries[indexPath.row],
                                                     coder: coder)
                }) else {
                return
            }
        ```
        
## β° νμλΌμΈ

<details>
<summary>Step 1 νμλΌμΈ</summary>
    
- **221018**
    - Asset μΆκ°
    - ExibitionEntry κ΅¬μ‘°μ²΄ κ΅¬ν
    - ExpositionUniverselle κ΅¬μ‘°μ²΄ κ΅¬ν
    - Step1 PR λ¦¬λ·° μμ²­
        - [PRλ³΄λ¬κ°κΈ°](https://github.com/yagom-academy/ios-exposition-universelle/pull/203)

</details>
    
<details>
<summary>Step 2 νμλΌμΈ</summary>   
    
- **221019**
    - λ©μΈνλ©΄ μ€ν¬λ‘€ λ·° λ μ΄μμ κ΅¬μ±, MainViewController IBOulet μ°κ²°
    - jsonνμΌμμ expoμ λ³΄λ₯Ό λΆλ¬μ€λ fetchExpoInformation λ©μλ κ΅¬ν
    - νλ©΄μ λ³΄μ¬μ§ νμ€νΈλ₯Ό μ€μ νλ setTextToDisplay() λ©μλ κ΅¬ν
    - νκ΅­μ μΆνμ KoreanEntriesViewController μμ±νκ³  IBOutlet μ€μ 
    - JSON νμΌμμ νκ΅­μ μΆνμμ λΆλ¬μ€λ fetchKoreanEntries() λ©μλ κ΅¬ν
    - KoreanEntriesViewController UITableViewDataSource required λ©μλ κ΅¬ν
    - μΆνμ μμΈ λ·° μ»¨νΈλ‘€λ¬ EntryDetailViewController κ΅¬ν λ° μμΈλ  μ°κ²°
    - KoreanEntriesViewController λ·° μ»¨νΈλ‘€λ¬μμ λνμΌ λ·° μ»¨νΈλ‘€λ¬λ‘ μ΄λνλ λ©μλ κ΅¬ν
    - EntryDetail Viewλ‘ λ°μ΄ν° μ λ¬μ μν prepare() λ©μλ κ΅¬ν
    - EntryDetailViewControllerμμ μμΈμ λ³΄λ₯Ό λ³΄μ¬μ£Όλ setViewToDisplay() λ©μλ κ΅¬ν
    
- **221020**
    - UIViewController verticalStackView height constraint μμ±
    - MainViewControllerμμ NavigationBar λνλμ§ μλλ‘ μμ 
    - νΉμ  νμ€νΈλ§ font ν¬κΈ° λ³κ²½κΈ°λ₯ attributedText μ΄μ©νμ¬ κ΅¬ν
    - MainViewControllerμμ λ°©λ¬Έμ μ NumberFormatterμ μ©
    - String+ createAttributed() λ©μλ κ΅¬ν
    - ExpoConstant name space μΆκ° λ° μμ 
    
- **221021**
    - JSONλμ½λ© μ½λ μ€λ³΅μ μ€μ΄κΈ° μν΄ JSONDecodingManager ν΄λμ€ κ΅¬ν
    - Step2 PR λ¦¬λ·° μμ²­
        - [PRλ³΄λ¬κ°κΈ°](https://github.com/yagom-academy/ios-exposition-universelle/pull/214)
    - String extension MainViewControllerλ‘ μ΄λνκ³  fileprivate μ€μ 
    - createAttributed() λ©μλ νμ₯μ±μ μν΄ νλΌλ―Έν° μμ 
    - λ°μ΄ν°λ₯Ό μλͺ»κ°μ Έμμ λ descriptionTextView.text μ€λ₯ λ©μΈμ§ νμ
    
</details>
 
<details>
<summary>Step 3 νμλΌμΈ</summary>
    
- **221026**
    - ExpositionUniverselleVCμμ μΈλ‘λͺ¨λλ§ μ§μνλλ‘ NavigationVC delegate κ΅¬ν
    - EntryTableViewCell κ΅¬ν λ° constraints μ½λλ‘ μ μ©
    - UIμμ Dynamic Type μ μ©
    - ExpositionUniverselleViewController μΈλ‘λ‘ κ³ μ λκ² μ½λ μΆκ°
    - Step3 PR λ¦¬λ·° μμ²­
        - [PRλ³΄λ¬κ°κΈ°](https://github.com/yagom-academy/ios-exposition-universelle/pull/232)

- **221027**
    - EntryTableViewCellμ reuseIdentifierλ₯Ό String literalμ μ¬μ©νμ§ μκ³  νμλͺμ μ¬μ©νλλ‘ μμ 
    - νΈμΆλΆκ° κΈΈμ΄μ§μ§ μλλ‘ `makeLabelString` λ©μλ μμ±νκ³  λ΄λΆμμ createAttributed() νΈμΆνλλ‘ μμ 
    - EntryDetailViewController νλ‘νΌν° private letμΌλ‘ λ³κ²½νκ³  μ΄λμλΌμ΄μ λ₯Ό μ΄μ©νμ¬ μμ±/μ°κ²°νλλ‘ μμ 
    - KoreanEntriesVCμμ indexPath.row νΈμΆ μ safe ν€μλ μ¬μ©νμ¬ subScript κ΅¬ν
    - μλ¬κ° λ°μνμ λ λμΈ alertλ₯Ό μμ±νλ showErrorAlert() λ©μλ κ΅¬ν
    
    
 </details>
    
## π± μ€ν νλ©΄

|λ§κ΅­λ°λν<br>1900 μ λ³΄|νκ΅­μ μΆνμ<br>μ λ³΄ νμ΄λΈ| μΆνμ μμΈνλ©΄ |
|:--:|:--:|:--:|
|![](https://i.imgur.com/li3xFxH.png)|![](https://i.imgur.com/u9Q3aqn.png)|![](https://i.imgur.com/IsMjcOl.png)|

- λ€μν μ¬μ΄μ¦μ iPhoneμ λμνλλ‘ Auto Layoutμ μ μ©νμμ΅λλ€.

|iPod touch|iPhone 12 mini|iPhone 13 Pro Max|
|:--:|:--:|:--:|
|![dVbw7k7](https://user-images.githubusercontent.com/85005933/198513623-db2532d3-071d-464c-8ea6-2a8c9eadfe58.gif)|![](https://i.imgur.com/D5UxXqn.gif)|![FXtTpTw](https://user-images.githubusercontent.com/85005933/198513651-6d794734-428c-4dfa-b88e-74a503a4d63c.gif)|



- μ²« λ²μ§Έ Viewμμλ μΈλ‘λͺ¨λλ§ μ§μνκ³  λ€λΉκ²μ΄μ λ°κ° λΈμΆλμ§ μκ³ , λλ¨Έμ§ Viewμμλ κ°λ‘/μΈλ‘ λͺ¨λλ₯Ό μ§μν©λλ€.
![WBnkhlU](https://user-images.githubusercontent.com/85005933/198513349-712d259b-0ca6-4de8-96d5-578da511c7ea.gif)

- Dynamic Typeμ μ μ©νμ¬ λλ°μ΄μ€μ κΈμ¨ ν¬κΈ° μ€μ μ μ μ©νμ¬ λ³΄μ¬μ€λλ€.
![G86DrVJ](https://user-images.githubusercontent.com/85005933/198513365-703a929e-470e-4b11-970d-c67bbbf1e654.gif)

- λ°μ΄ν° νμ±μ μ€ν¨νμ λ μ¬μ©μμκ² alertλ₯Ό μ΄μ©νμ¬ μ€ν¨νμμμ λ³΄μ¬μ€λλ€.
<center><img src = "https://i.imgur.com/PtRmRmt.png" width=200></center>

## β νΈλ¬λΈ μν

### Step 1

- STEP 1μ JSON ν¬λ§·μ λ°μ΄ν°μ λ§€μΉ­λλ λͺ¨λΈ νμμ κ΅¬ννλ κ°λ¨ν μκ΅¬μ¬ν­μ΄μ΄μ νΈλ¬λΈ μν λ΄μ©μ΄ μμ΅λλ€.

### Step 2

- ν νλ©΄μμ λ€λΉκ²μ΄μ λ°λ₯Ό λΈμΆλμ§ μκ² νλ λ°©λ²
   - `self.navigationController?.isNavigationBarHidden = true`λ₯Ό viewDidLoad() λ©μλμμ μ¬μ©νμ¬ λ€λΉκ²μ΄μ λ°λ₯Ό λΈμΆλμ§μκ² ν΄λ³΄μμ λ κ°μ κ³μΈ΅μμλ Viewλ€ μ λΆ λ€λΉκ²μ΄μ λ°κ° λΈμΆλμ§μλ λ¬Έμ κ° λ°μνμμ΅λλ€.
   - `self.navigationController?.isNavigationBarHidden = false`λ₯Ό ν νλ©΄μ΄ μ¬λΌμ§ λ μ¬μ©νμ¬ λ€μ λ€λΉκ²μ΄μ λ°κ° λνλ  μ μκ² κ΅¬νν΄λ³΄μμ΅λλ€.
   - ν΄λΉ μ½λλ₯Ό viewDidAppearμμ λ€λΉκ²μ΄μ λ°κ° λ€μ λνλλ μμ μ΄ λ€μ Viewλ‘ pushλ νμ λνλκ² λμ΄μ μ΄λ₯Ό ν΄κ²°νκΈ° μν΄ viewWillAppearμμ ν΄λΉ μ½λλ₯Ό μ¬μ©νμμ΅λλ€.
   
- JSONDecodingManager νμμ κ΅¬νν  λ μ¬λ¬ νμμ κ°μ λμ½λ©ν  μ μκ² κ΅¬ννκΈ°
    - JSONDecoderλ₯Ό μμ±νκ³  decode λ©μλλ₯Ό ν΅ν΄μ λμ½λ©νλ μ½λκ° μ€λ³΅λμ΄μ ν΄λΉ κΈ°λ₯μ λ¬Άμ΄μ£Όλ μμμ νμμ΅λλ€.
    - ν΄λΉ κΈ°λ₯μ λ¬Άμμ λ μ¬λ¬κ°μ§ νμμΌλ‘ λμ½λ©λμ΄μΌ νλ κΈ°λ₯μ μ΄λ»κ² κ΅¬νν΄μΌ ν μ§ κ³ λ―Όνμμ΅λλ€.
    - ν΄λΉ λ¬Έμ λ₯Ό μ λ€λ¦­νμμ μ΄μ©νμ¬ μ¬λ¬ νμμ λμν  μ μκ² κ΅¬ννμμ΅λλ€.
    ```swift
    func decode<T: Decodable>(dataAsset: String) throws -> T {
        guard let dataAsset: NSDataAsset = NSDataAsset(
            name: dataAsset) else {
            throw ExpoError.dataAssetError
        }
        
        let data = try jsonDecoder.decode(T.self, from: dataAsset.data)
        
        return data
    }
    ```

- ννλ©΄μμ "κ°μ΅μ§ : νλμ€ νλ¦¬" λ±μΌλ‘ λ μ΄λΈ νμ€νΈμ JSONμμ κ°μ Έμ¨ λ°μ΄ν°λ₯Ό ν¨κ» λ³΄μ¬μ€ λ ν°νΈ μ¬μ΄μ¦λ₯Ό μ²λ¦¬νλ λ°©μ
    - κ°λ¨ν λ°©λ²μΌλ‘λ Labelμ 2κ°λ‘ λλκ³ , κ°κ°μ λ μ΄λΈ νμ€νΈλ₯Ό λ€λ₯Έ ν¬κΈ°λ‘ μ£Όμ΄ ν΄κ²°ν  μ μμμ§λ§, λ°©λ²μ μ°Ύμλ³΄λ μ€μ `attributedString`μ λν΄ μκ² λμκ³  μ΄λ² νλ‘μ νΈμμ μ μ©ν΄ λ³΄μμ΅λλ€.
    - μ²μ μλν λ°©λ²
    ```swift
        let fontSize = UIFont.systemFont(ofSize: 20)

        let location: String = "κ°μ΅μ§ : " + expositionUniverselle.location
        let locationAttributed = NSMutableAttributedString(string: location)
        let locationRange = (location as NSString).range(of: "κ°μ΅μ§")

        locationAttributed.addAttribute(.font, value: fontSize, range: locationRange)

        locationLabel.text = "κ°μ΅μ§ : " + expositionUniverselle.location
        locationLabel.attributedText = locationAttributed
    ```
    - λ¦¬ν©ν λ§ μ String extensionμμ λ©μλλ‘ μ²λ¦¬
    ```swift
     func createAttributed(target: String) -> NSAttributedString {
        let fontSize = ExpoConstant.mediumFont
        let attributed: NSMutableAttributedString = NSMutableAttributedString(string: self)
        let targetRange = (self as NSString).range(of: target)
        attributed.addAttribute(.font, value: fontSize, range: targetRange)
        
        return attributed
    }
    ```

### Step 3

- μ²«λ²μ§Έ Viewλ§ μΈλ‘λͺ¨λλ‘ κ³ μ νκΈ° μν λ°©λ²
    - ExpositionUniverselleViewControllerμμ navigationViewControllerμ delegateλ₯Ό selfλ‘ μ§μ ν ν
        ```swift
        func navigationControllerSupportedInterfaceOrientations(
        _ navigationController: UINavigationController
        )
        ```
        λ©μλλ₯Ό κ΅¬ννμ¬ μ¬μ μν ` supportedInterfaceOrientations`μ λ¦¬ν΄νμ¬ κ° νλ©΄λ§λ€ μ§μνλ λ°©ν₯μ μ€μ ν΄μ£Όμμ΅λλ€.
    - μ΄μΈμλ UINavigationControllerμ subClassλ₯Ό κ΅¬ννμ¬ ` supportedInterfaceOrientations`λ₯Ό μ¬μ μνλ λ°©λ²κ³Ό AppDelegateμ λ©μλμΈ 
        ```swift
        func application(_ application: UIApplication, supportedInterfaceOrientationsFor window: UIWindow?) -> UIInterfaceOrientationMask
        ```
        λ₯Ό κ΅¬ννμ¬ μ€μ ν΄μ£Όλ λ°©λ²μ ν¨κ» κ³ λ―Όνμμ΅λλ€.
        
    - μ²μμλ ExpositionUniverselleViewControllerμ `viewDidLoad`μμ λ©μλλ₯Ό νΈμΆνμλ€κ° λ€μ Viewλ‘ λμ΄κ°λ€κ° λ€μ λμμ€λ κ²½μ°μ μ²«λ²μ§Έ Viewκ° κ°λ‘λ‘ νμ νλ λ¬Έμ κ° μμλλ° `viewWillAppear`λ‘ μ΄λν ν ν΄κ²°λμμ΅λλ€.
        
- μ²«λ²μ§Έ Viewμμ μλ?¬λ μ΄ν°λ₯Ό κ°λ‘λ‘ λνκ³  λ€μ Viewλ‘ μ ννμμ λ λλ²μ§Έ Viewκ° Landscapeλ‘ presentλμ§ μμ
    - νμ¬ λλ°μ΄μ€μ λ¬Όλ¦¬μ μΈ λ°©ν₯μ μ½μ΄μμ Viewκ° νμλμμ λ κ·Έ κ°μ κΈ°μ€μΌλ‘ λ°©ν₯μ μ ν΄μ£Όκ³  μΆμλλ° Landscape leftμ rightλ₯Ό κ΅¬λΆνλ κ²μ μ€ν¨νμ΅λλ€.  
    ![](https://i.imgur.com/GDqqJ8d.gif)
    - νμ¬ μνμ μ½λμμ `XCode 14` λ²μ μ μ¬μ©νκ³  μλ λ¦¬λ·°μ΄μ λ€λ₯Έ μΊ νΌλ€μ ν΄λΉ νμμ΄ λνλμ§ μκ³  κ°λ‘λ‘ λν μνμμ λ€μ Viewλ‘ μ΄λνλ©΄ Landscapeλ‘ λ³κ²½λμ΄ λΈμΆλλ€κ³  ν΄μ `XCode 13` λ²μ μ λ²κ·Έμ΄μ§ μμκΉ..λ‘ λ§λ¬΄λ¦¬ λμμ΅λλ€.

- AttributedStringμ Dynamic Type μ μ© μ, νμͺ½λ§ μ μ©λλ λ¬Έμ 
    - Dynamic Typeμ μ μ©νκ³  νμΈν΄ λ³΄λ AttributedStringμ΄ μ μ©λ Textμλ§ Dynamic Typeμ΄ μ μ©λκ³  λ€μͺ½ Textμλ μ μ©λμ§ μλ λ¬Έμ κ° μμμ΅λλ€.
    - [μ νλ¬Έμ](https://developer.apple.com/documentation/uikit/uilabel/1620542-attributedtext)μμ attributedTextκ° μ μ©λλ μμ μ μ²« λ²μ§Έ λ¬Έμμ μ€νμΌ μ λ³΄λ‘ UILableμ μ€νμΌ κ΄λ ¨ νλ‘νΌν°λ₯Ό μλ°μ΄νΈ νλ κ²μΌλ‘ μ΄μΌκΈ° νκ³  μμ΄μ, `createAttributed` λ©μλμμ 2κ°μ parameterλ₯Ό λ°μ zip ν¨μλ₯Ό μ΄μ©ν΄μ κ°κ° λ€λ₯Έ ν¬κΈ°λ‘ AttributeStringμ λ§λ€κ³  ν©μ³μ λ³΄μ¬μ£Όλλ‘ κ΅¬ννμμ΅λλ€.

- μ²«λ²μ§Έ View νλ¨ `νκ΅­μ μΆνμ λ³΄λ¬κ°κΈ°` λ²νΌμ Dynamic Type μ μ© μ , μ€νλ·°λ₯Ό λ²μ΄λμ λΈμΆλλ λ¬Έμ 
    - ν΄λΉ λ²νΌμ΄ μν΄μλ μ€νλ·°μ λμ΄κ° 50μΌλ‘ μ§μ λμ΄ μμ΄μ Dynamic Typeλ₯Ό μ μ©νμ λ νμ€νΈκ° λ²νΌμ μ¬μ΄μ¦λ₯Ό λ²μ΄λμ λΈμΆλμμ΅λλ€.
    - ν΄λΉ μ€νλ·°μ λμ΄ μ μ½ μ‘°κ±΄μ μ§μ°λ©΄ μ€νλ·°μ λμ΄κ° λμ΄λλ λ¬Έμ κ° λ°μνμ΅λλ€.
    <center><img src="https://i.imgur.com/41mQaCk.png" width="300" height="300"></center>
    
    - μ΄ λ¬Έμ λ₯Ό ν΄κ²°νκΈ° μν΄μ λ²νΌμ `Hugging Priority`λ₯Ό 1000μΌλ‘ μ£Όμ΄μ λμ΄λμ§ μλλ‘ νμ¬ ν΄κ²°νμμ΅λλ€.

|μμ  μ |μμ  ν|
|:--:|:--:|
|![](https://i.imgur.com/yVctJUP.png)|![](https://i.imgur.com/NJMbkyE.png)|


## π μ°Έκ³  λ§ν¬

[Swift Doc - UITableView](https://developer.apple.com/documentation/uikit/uitableview)   
[Swift Doc - Table views](https://developer.apple.com/documentation/uikit/views_and_controls/table_views)  
[Filling a table with data](https://developer.apple.com/documentation/uikit/views_and_controls/table_views/filling_a_table_with_data)  
[Configuring the cells for your table](https://developer.apple.com/documentation/uikit/views_and_controls/table_views/configuring_the_cells_for_your_table)  
[prepareForReuse()](https://developer.apple.com/documentation/uikit/uitableviewcell/1623223-prepareforreuse)  
[JSONDecoder](https://developer.apple.com/documentation/foundation/jsondecoder)  
[Using JSON with Custom Types](https://developer.apple.com/documentation/foundation/archives_and_serialization/using_json_with_custom_types)  
[Encoding and Decoding Custom Types](https://developer.apple.com/documentation/foundation/archives_and_serialization/encoding_and_decoding_custom_types)  
[WWDC2017 - Modern cell configuration](https://developer.apple.com/videos/play/wwdc2020/10027/)  
[iOS λΆμ€νΈμ½μ€ - κΈ°μμ λ³΄ μ νλ¦¬μΌμ΄μ](https://www.boostcourse.org/mo326/joinLectures/12973?isDesc=false)  
[Labelμ λΆλΆ κΈμ ν¬κΈ°/ν°νΈ/μμ λ³κ²½λ°©λ²](https://zeddios.tistory.com/m/300)  
[WWDC 2019 - Accessibility Inspector ](https://developer.apple.com/videos/play/wwdc2019/257/)  
[WWDC 2019 - Writing Great Accessibility Labels ](https://developer.apple.com/videos/play/wwdc2019/254/)  
[Easy to Use Cell Reuse Extensions](https://stephenfeuerstein.com/tutorials/easy-to-use-cell-reuse-extensions)  
[Safe (bounds-checked) array lookup in Swift](https://stackoverflow.com/questions/25329186/safe-bounds-checked-array-lookup-in-swift-through-optional-bindings/30593673#30593673)  

---

[π λ§¨ μλ‘ μ΄λνκΈ°](#-λ§κ΅­λ°λν)
