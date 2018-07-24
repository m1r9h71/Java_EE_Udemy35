# Java_EE_Udemy35
Adding Pilots to Flight - One To Many Relashionship completed
Inside AddPilotToFlight Servlet:

      String pid = request.getParameter("pid");
		  String fid = request.getParameter("fid");
		
		  fs.addPilotToFlight(pid, fid);
      
Inside FlightService:
      
       List<Pilot> pList = f.getPilots();
    	
    	pList.add(p);
    	
    	f.setPilots(pList);
    	
    	p.setFlightForPilot(f);
