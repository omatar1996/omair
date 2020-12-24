import 'package:flutter/material.dart';

class GsG extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    // TODO: implement build
    return DefaultTabController(
      length: 2,
      child: Scaffold(
        body: Column(
          children: [
            Container(
              height: 300,
              color: Colors.black,
            ),
            Container(
              color: Colors.red,
              height: 50,
              child: TabBar(indicatorColor: Colors.blue, tabs: [
                Tab(
                  child: Text('Posts', style: TextStyle(color: Colors.black)),
                ),
                Tab(
                  child: Text('Likes', style: TextStyle(color: Colors.black)),
                )
              ]),
            ),
            Expanded(
              child: TabBarView(children: [
                Center(
                  child: Text('Sammy'),
                ),
                Center(
                  child: Text('Khaled'),
                )
              ]),
            )
          ],
        ),
      ),
    );
  }
}
