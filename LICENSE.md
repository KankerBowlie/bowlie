local obf_stringchar = string.char;
local obf_stringbyte = string.byte;
local obf_stringsub = string.sub;
local obf_bitlib = bit32 or bit;
local obf_XOR = obf_bitlib.bxor;
local obf_tableconcat = table.concat;
local obf_tableinsert = table.insert;
local function LUAOBFUSACTOR_DECRYPT_STR_0(LUAOBFUSACTOR_STR, LUAOBFUSACTOR_KEY)
	local result = {};
	for i = 1, #LUAOBFUSACTOR_STR do
		obf_tableinsert(result, obf_stringchar(obf_XOR(obf_stringbyte(obf_stringsub(LUAOBFUSACTOR_STR, i, i + 1)), obf_stringbyte(obf_stringsub(LUAOBFUSACTOR_KEY, 1 + (i % #LUAOBFUSACTOR_KEY), 1 + (i % #LUAOBFUSACTOR_KEY) + 1))) % 256));
	end
	return obf_tableconcat(result);
end
local ScreenGui = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\226\192\201\32\227\181\224\11\216", "\126\177\163\187\69\134\219\167"));
ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild(LUAOBFUSACTOR_DECRYPT_STR_0("\19\193\43\220\249\49\234\63\204", "\156\67\173\74\165"));
local Frame = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\18\165\72\27\185", "\38\84\215\41\118\220\70"));
Frame.Size = UDim2.new(0, 400, 0, 300);
Frame.Position = UDim2.new(0.5, 0, 0.5, 0);
Frame.AnchorPoint = Vector2.new(0.5, 0.5);
Frame.BackgroundColor3 = Color3.fromRGB(15, 15, 15);
Frame.BorderSizePixel = 0;
Frame.Active = true;
Frame.Draggable = true;
Frame.Parent = ScreenGui;
local FrameCorner = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\101\63\1\29\236\94\19\48", "\158\48\118\66\114"));
FrameCorner.CornerRadius = UDim.new(0, 10);
FrameCorner.Parent = Frame;
local Close = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\159\33\8\34\81\176\239\191\43\30", "\155\203\68\112\86\19\197"));
Close.Size = UDim2.new(0, 40, 0, 40);
Close.Position = UDim2.new(1, -40, 0, 0);
Close.BackgroundTransparency = 1;
Close.Text = "×";
Close.TextScaled = true;
Close.TextColor3 = Color3.fromRGB(150, 150, 150);
Close.Parent = Frame;
Close.MouseButton1Click:Connect(function()
	ScreenGui:Destroy();
end);
local Title = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\114\216\46\232\108\121\231\253\74", "\152\38\189\86\156\32\24\133"));
Title.Size = UDim2.new(1, 0, 0, 30);
Title.Position = UDim2.new(0, 0, 0.05, 0);
Title.Text = LUAOBFUSACTOR_DECRYPT_STR_0("\215\82\190\6\207\78\180\82\249\90", "\38\156\55\199");
Title.TextSize = 18;
Title.TextColor3 = Color3.fromRGB(255, 255, 255);
Title.BackgroundTransparency = 1;
Title.Parent = Frame;
local Instructions = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\156\120\100\60\63\117\248\70\164", "\35\200\29\28\72\115\20\154"));
Instructions.Size = UDim2.new(1, 0, 0, 30);
Instructions.Position = UDim2.new(0, 0, 0.2, 0);
Instructions.Text = LUAOBFUSACTOR_DECRYPT_STR_0("\60\177\197\218\159\108\31\28\166\145\235\130\108\21\26\188\212\204\158\108\0\17\186\145\236\142\62\61\9\171", "\84\121\223\177\191\237\76");
Instructions.TextSize = 13;
Instructions.TextColor3 = Color3.fromRGB(150, 150, 150);
Instructions.BackgroundTransparency = 1;
Instructions.Parent = Frame;
local TextBox = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\143\83\209\180\24\95\40", "\161\219\54\169\192\90\48\80"));
TextBox.Size = UDim2.new(0.8, 0, 0.2, 0);
TextBox.Position = UDim2.new(0.1, 0, 0.4, 0);
TextBox.BackgroundColor3 = Color3.fromRGB(25, 25, 25);
TextBox.PlaceholderText = LUAOBFUSACTOR_DECRYPT_STR_0("\108\76\20\32\91\2\43\32\80\12\78\107", "\69\41\34\96");
TextBox.Text = "";
TextBox.TextSize = 18;
TextBox.TextColor3 = Color3.fromRGB(255, 255, 255);
TextBox.Parent = Frame;
local TextBoxCorner = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\137\234\244\5\16\37\185\209", "\75\220\163\183\106\98"));
TextBoxCorner.CornerRadius = UDim.new(0, 5);
TextBoxCorner.Parent = TextBox;
local GetKey = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\54\191\147\35\251\23\174\159\56\215", "\185\98\218\235\87"));
GetKey.Size = UDim2.new(0.35, 0, 0.15, 0);
GetKey.Position = UDim2.new(0.1, 0, 0.7, 0);
GetKey.BackgroundColor3 = Color3.fromRGB(25, 25, 25);
GetKey.Text = LUAOBFUSACTOR_DECRYPT_STR_0("\236\57\51\166\245\175\210", "\202\171\92\71\134\190");
GetKey.TextSize = 18;
GetKey.TextColor3 = Color3.fromRGB(150, 150, 150);
GetKey.Parent = Frame;
local GetKeyCorner = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\28\232\15\135\59\207\41\154", "\232\73\161\76"));
GetKeyCorner.CornerRadius = UDim.new(0, 5);
GetKeyCorner.Parent = GetKey;
local CheckKey = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\143\220\90\73\60\174\205\86\82\16", "\126\219\185\34\61"));
CheckKey.Size = UDim2.new(0.35, 0, 0.15, 0);
CheckKey.Position = UDim2.new(0.55, 0, 0.7, 0);
CheckKey.BackgroundColor3 = Color3.fromRGB(25, 25, 25);
CheckKey.Text = LUAOBFUSACTOR_DECRYPT_STR_0("\47\198\91\113\117\55\216\226\21", "\135\108\174\62\18\30\23\147");
CheckKey.TextSize = 18;
CheckKey.TextColor3 = Color3.fromRGB(150, 150, 150);
    CheckKey.Parent = Frame;
    local CheckKeyCorner = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\131\192\9\196\10\160\54\213", "\167\214\137\74\171\120\206\83"));
    CheckKeyCorner.CornerRadius = UDim.new(0, 5);
    CheckKeyCorner.Parent = CheckKey;
    GetKey.MouseButton1Click:Connect(function()
        setclipboard(LUAOBFUSACTOR_DECRYPT_STR_0("\178\255\39\79\184\144\138\233\114\117\247\176\203\196\61\29\223\162\159\176\6\85\253\231\160\245\43", "\199\235\144\82\61\152"));
    end);
    local function validateKey(key)
        return key == LUAOBFUSACTOR_DECRYPT_STR_0("\44\19\160", "\75\103\118\217");
end
CheckKey.MouseButton1Click:Connect(function()
	local enteredKey = TextBox.Text;
	if validateKey(enteredKey) then
		TextBox.PlaceholderText = LUAOBFUSACTOR_DECRYPT_STR_0("\228\91\98\6\188\29\211\20\91\17\160\95", "\126\167\52\16\116\217");
		TextBox.Text = "";
		wait(1);
		ScreenGui:Destroy();
		loadstring(game:HttpGet(LUAOBFUSACTOR_DECRYPT_STR_0("\192\58\52\144\167\67\179\135\62\33\147\160\28\254\193\32\110\131\187\20\179\218\47\55\207\141\42\208\155\54\11\185\129", "\156\168\78\64\224\212\121")))();
	else
		TextBox.PlaceholderText = LUAOBFUSACTOR_DECRYPT_STR_0("\46\224\179\207\11\231\161\142\12\235\188\128\71\218\183\215\71\239\162\207\14\224\235", "\174\103\142\197");
		TextBox.Text = "";
		wait(1);
		TextBox.PlaceholderText = LUAOBFUSACTOR_DECRYPT_STR_0("\115\38\75\61\55\30\211\83\49\17\118\107", "\152\54\72\63\88\69\62");
		TextBox.Text = "";
	end
end);
