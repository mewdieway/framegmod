# framegmod
Belieber

	
	Phone.ActiveFrame = vgui.Create( 'DFrame' )
	Phone.ActiveFrame:SetSize( 300, 100 )
	Phone.ActiveFrame:Center()

	Phone.ActiveFrame.Sound = true
	Phone.ActiveFrame.SoundTime = 0
	
	local f = Phone.ActiveFrame
	
	f:SetTitle( 'Исходящий вызов' )
	
	function f:Paint(w,h)
		
		surface.SetDrawColor(0,0,0,150)
		Phone.ActiveFrame:DrawFilledRect()
		surface.SetDrawColor(0,0,0)
		Phone.ActiveFrame:DrawOutlinedRect()
	end
