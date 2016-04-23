	
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
	
		slb = vgui.Create( "DButton", Phone.ActiveFrame )
	slb:SetSize( 110, 20 ) 
	slb:SetPos( 185, 68 )
	slb:SetText( "Leave" )
	slb:SetImage( "icon16/comments_delete.png" )
	slb:SetTextColor( Color(255,255,255) )
	slb.Paint = function() 
		surface.SetDrawColor(0,0,0)
		slb:DrawOutlinedRect()
	end
